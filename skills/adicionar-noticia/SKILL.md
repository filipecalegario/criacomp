# Skill: Adicionar Notícia via Telegram

Use esta skill quando o usuário enviar uma notícia no Telegram (qualquer link na conversa) para adicionar automaticamente no arquivo de news do repositório e abrir um PR para o upstream.

## Quando ativar

Sempre que a mensagem do usuário no Telegram contiver um link de notícia (URL válida). A skill é acionada automaticamente pelo agente quando detecta uma URL na mensagem.

## Fluxo de automação

### Passo 1: Extrair informações da notícia

- **URL**: a URL enviada pelo usuário (obrigatória)
- **Título**: usar o título que o usuário forneceu na mensagem, ou tentar extrair da URL se não houver
- **Data**: data de hoje no formato `DD/MM/AAAA`

Se o usuário enviou apenas a URL sem título, o agente deve:
1. Tentar extrair o título da página (opcional — o CLAUDE.md diz para registrar com o título que o usuário forneceu; se não houver, usar um título neutro como "Link enviado por [usuário]")
2. Registrar com o título recebido

### Passo 2: Editar o arquivo de news

Arquivo-alvo: `2026-2-NEWS.md` (está na raiz do repositório)

Regras (baseadas no CLAUDE.md do repositório):

1. **Ordem**: a data mais recente fica no **topo** do arquivo
2. **Seção de data**: `## DD/MM/AAAA` no topo. Se já existir seção com hoje, usar essa; se não, criar no topo
3. **Formato do item**: `- [título](url)` — lista não ordenada Markdown
4. **Título**: usar o título que o usuário forneceu. Não traduzir, não reescrever
5. **Subtópicos**: se houver notícias relacionadas, indentar com 2 espaços
6. **Sem comentários no NEWS**: apenas links, sem resumo

Exemplo de como o arquivo deve ficar após adicionar:

```markdown
## 08/09/2026

- [Título da Notícia Enviada](https://exemplo.com/noticia)
- [Outra notícia...](https://outro-lugar.com)

## 01/09/2026  ← seção existente permanece abaixo
...
```

### Passo 3: Commit e push

1. Criar branch com nome descritivo: `news/YYYY-MM-DD-slug` (ex: `news/2026-09-08-ferramenta-ia-cardiaca`)
2. Commit com mensagem no formato: `add: <título curto da notícia>`
3. Push para o fork (`origin`): `git push -u origin <branch-name>`

### Passo 4: Abrir PR para o upstream

```bash
gh pr create \
  --base main \
  --head JosiasNetto:<branch-name> \
  --title "add: <título curto da notícia>" \
  --body "## Summary\n\n- Adiciona notícia: <título>\n- Link: <url>\n- Data: <DD/MM/AAAA>\n\n## Test Plan\n\n- [ ] Verificar formatação no NEWS"
```

O PR deve apontar para `filipecalegario/criacomp` (upstream), com base `main`.

### Passo 5: Informar o resultado ao usuário

Responder no Telegram com:
- Link do PR criado
- Resumo do que foi adicionado

Se falhar, informar o erro claro.

## Variáveis de ambiente e dependências

- `gh` CLI autenticado com token `repo` scope
- Git configurado com SSH ou HTTPS para o fork
- Remote `upstream` configurado apontando para `https://github.com/filipecalegario/criacomp.git`

## Exemplos de uso

### Exemplo 1: Usuário envia URL com título

```
Usuário: https://www.example.com/noticia - "Novas perspectivas em IA generativa"
```

Fluxo:
1. Título: "Novas perspectivas em IA generativa"
2. URL: https://www.example.com/noticia
3. Adiciona no topo com `## 08/09/2026` (se for hoje)
4. PR para upstream

### Exemplo 2: Usuário envia apenas URL

```
Usuário: https://techcrunch.com/2026/09/08/ai-launches
```

Fluxo:
1. Título: usar o título da página (se possível) ou "Link enviado por Josias"
2. Restante igual

## Cuidados

- Nunca adicionar no final do arquivo — sempre no topo
- Se já existir seção `## DD/MM/AAAA` para hoje, adicionar items nela, não criar duplicata
- Não abrir PRs duplicados para a mesma notícia
- Se o PR já existe para o mesmo link, informar ao usuário em vez de criar novo
