# CLAUDE.md

Repositório da disciplina **Criatividade Computacional (IF866)** — Centro de Informática, UFPE.

Edição atual: **2026.2**

## Estrutura do repositório

- `2026-2-NEWS.md` — notícias da edição corrente (2026.2)
- `2026-2-NOTES.md` — comentários e contexto sobre os links do NEWS da edição corrente
- `ARCHIVED/` — notícias e notebooks de edições anteriores, com o padrão de nome antigo (`2023_2_news.md`, `2024_1_news.md`, `2024_2_news.md`, `2025_1_news.md`, ...)
- `README.md` — apresentação da disciplina, avaliação e projetos de períodos anteriores. Traz, logo no início, o link e a descrição do arquivo de notícias da edição corrente — **atualizar esse bloco a cada nova edição**.
- `PROMPT_COLLECTION.md` — coleção de prompts usados em aula
- `embeddings/`, `primeiros-passos/` — notebooks e materiais práticos

## Padrão para adicionar notícias

As notícias são links compartilhados e discutidos no início de cada aula ("descobertas da semana"). Elas vivem no arquivo de notícias da edição corrente — hoje, `2026-2-NEWS.md`.

### Regras

1. **Arquivo**: sempre o da edição corrente, nomeado `<ANO>-<SEMESTRE>-NEWS.md` (ex.: `2026-2-NEWS.md`). Ao virar o semestre, mover o arquivo antigo para `ARCHIVED/` e criar o novo.
   - Esse padrão de nome foi **definido em 20/08/2026, a partir da edição 2026.2**. Os arquivos anteriores permanecem com o nome antigo (`<ANO>_<SEMESTRE>_news.md`, ex.: `ARCHIVED/2025_1_news.md`) — **não renomear**. A convenção nova vale só daqui pra frente.
2. **Ordem cronológica inversa**: a data mais recente fica no **topo** do arquivo. Nunca acrescentar no fim.
3. **Cabeçalho de data**: `## DD/MM/AAAA` (dia/mês/ano, com zeros à esquerda). Uma seção por dia de aula.
   - Se já existir uma seção com a data de hoje, adicionar os itens nela; caso contrário, criar uma nova seção no topo.
4. **Itens**: um link por linha, em lista não ordenada com `-`, no formato Markdown `- [título](url)`.
   - O **título é o título da página** (normalmente colado direto do navegador, inclusive quando vem longo ou com sufixos como `- InfoQ`, `/ X`, `\ Anthropic`). Manter como veio; não reescrever nem traduzir.
   - Links soltos sem título (`- https://...`) são aceitáveis para posts de Instagram/redes sociais quando não há título útil.
5. **Subtópicos**: uma notícia relacionada a outra entra **indentada com 2 espaços** sob o item principal, mantendo o mesmo formato de link.

   ```markdown
   - [Notícia principal](https://exemplo.com)
     - [Notícia relacionada / contraponto](https://exemplo.com/relacionada)
   ```
6. **Sem comentários editoriais no NEWS**: o arquivo é uma lista curada de links, não um resumo. Comentário, contexto e resumo vão para o arquivo de notes da edição (ver abaixo).

   > ⚠️ Nunca usar a palavra "notas" para esses arquivos ou links — confunde com nota/avaliação dos alunos. Sempre **notes**.
7. Não verificar/abrir os links por padrão — registrar o que o usuário forneceu, com o título que ele forneceu.

### Exemplo

```markdown
## 20/08/2026

- [guillaumemeyer/watermarks-remover: Strip multi-vendor AI provenance marks...](https://github.com/guillaumemeyer/watermarks-remover)
  - [How Claude's text watermarking works \ Anthropic](https://www.anthropic.com/news/claude-text-watermark)
- [SpaceXAI Launches Grok Bot for Autonomous AI Agents - InfoQ](https://www.infoq.com/news/2026/08/grok-bot-agent/)
```

## Comentários sobre as notícias (arquivo de notes)

Quando um link merece resumo, contexto ou pauta de discussão, isso **não** entra no NEWS. Vai para `<ANO>-<SEMESTRE>-NOTES.md` (ex.: `2026-2-NOTES.md`), que acompanha o NEWS da edição e é arquivado junto com ele no fim do semestre.

- Terminologia: sempre **notes**, nunca "notas" — evita confusão com nota/avaliação dos alunos.
- Um `##` por item comentado, com o mesmo título do link no NEWS. Abaixo do título, uma linha de procedência: fonte/autores + a data em que o link entrou no NEWS.
- Ordem cronológica inversa, igual ao NEWS.
- Fechar com um parágrafo **Para discutir em aula:** quando houver pauta — é o que o item rende de discussão, não o resumo de novo.
- No NEWS, o item comentado ganha **um** subtópico apontando para a âncora:

  ```markdown
  - [Título da notícia](https://exemplo.com)
    - [📝 notes](2026-2-NOTES.md#ancora-do-titulo)
  ```

  A âncora segue a regra do GitHub: minúsculas, espaços viram `-`, pontuação sai (`MatrAIx: Simulating the World with 8.3 Billion Persona Agents` → `#matraix-simulating-the-world-with-83-billion-persona-agents`).
- Só os itens que valem comentário ganham a linha. A maioria dos links fica sem, e tudo bem.

Este padrão de notes foi **definido em 20/08/2026, na edição 2026.2**. Edições anteriores não têm arquivo equivalente.
