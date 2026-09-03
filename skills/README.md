# Skills do Projeto Autoral

Quatro skills para os grupos da disciplina **Criatividade Computacional (IF866)** usarem durante o Projeto Autoral. Elas não fazem o projeto de vocês. Elas fazem vocês decidirem.

| skill | o que faz | quando usar |
|---|---|---|
| [`abrir-o-leque`](abrir-o-leque/SKILL.md) | gera possibilidades que vocês não teriam sozinhos | passo 1, quando o grupo está em branco ou preso no óbvio |
| [`afiar-o-eixo`](afiar-o-eixo/SKILL.md) | entrevista o grupo até o eixo ficar específico | passo 3, depois de escolher uma direção |
| [`derrubar-a-ideia`](derrubar-a-ideia/SKILL.md) | ataca a ideia já formada, procurando o ponto fraco | quando o eixo está escrito e o grupo acha que está pronto |
| [`escutar-a-reuniao`](escutar-a-reuniao/SKILL.md) | transforma a gravação de uma reunião do grupo em material de trabalho | depois de qualquer discussão longa |

## Como instalar

As skills são Markdown puro. Não dependem de nenhum agente específico, e é de propósito: nenhuma entrega desta disciplina pode exigir uma ferramenta em particular.

**Claude Code**

```bash
git clone https://github.com/filipecalegario/criacomp.git
mkdir -p .claude/skills
cp -R criacomp/skills/* .claude/skills/
```

Depois, `/afiar-o-eixo` (ou o nome de qualquer uma delas).

**OpenCode e outros agentes que leem `.agents/`**

```bash
mkdir -p .agents/skills
cp -R criacomp/skills/* .agents/skills/
```

**Qualquer chat, sem instalar nada**

Abra o `SKILL.md` da skill que você quer, copie o conteúdo inteiro e cole como primeira mensagem da conversa. Funciona igual. As skills foram escritas para sobreviver a esse caminho, que é o piso.

## Como usar

**Rodem sozinhos antes de rodar em grupo.** Se as cinco pessoas rodam a `abrir-o-leque` juntas, a primeira opinião dita em voz alta ancora todo mundo, que é exatamente o que estas skills existem para evitar. Cada um roda sozinho, depois vocês comparam o que saiu. Custa nada e multiplica o material.

**Registrem o uso no caderno de bordo.** Quatro linhas bastam: qual skill, quando usaram, o que ela mudou no que vocês estavam fazendo, e onde ela atrapalhou.

"Atrapalhou" é resposta boa. Se doze grupos escreverem "ajudou bastante", ninguém aprende nada sobre as skills, inclusive quem as escreveu. O relato de onde uma delas travou o grupo vale mais do que o elogio.

## A regra que atravessa as quatro

Nenhuma destas skills escreve o seu projeto. Elas perguntam, provocam e criticam, e param antes da decisão. Se você pedir a qualquer uma delas "então escreve o eixo pra mim", a resposta correta dela é recusar e devolver a pergunta.

Isso não é implicância. O que a disciplina avalia é o critério de vocês, e critério terceirizado não sobrevive à primeira pergunta da apresentação.

## Sobre gravar as reuniões

A skill `escutar-a-reuniao` existe porque gravar a discussão do grupo e processá-la com um agente é, hoje, um dos métodos mais úteis de concepção de projeto. A discussão de vocês é o material mais rico que o projeto produz, e é o único que evapora.

**A gravação é de vocês.** Não há obrigação de gravar, nada é entregue, e o professor não vai pedir a gravação nem a transcrição em nenhum momento. Se algo que saiu da reunião aparecer no caderno de bordo, é porque vocês decidiram colocar, com as palavras de vocês.

A skill roda na máquina do grupo, sobre um arquivo do grupo. Combinem entre vocês antes de ligar o gravador, e desliguem quando alguém pedir.

## Melhorar as skills

Se alguma delas estiver ruim, mande pull request. Vocês já têm este repositório clonado por causa do CriaComp News.

Melhoria aceita conta como **Experimento** no Portfólio, desde que venha com a Peça correspondente: o que você quis mudar, o que testou, o que aconteceu, o que aprendeu.

## Vocabulário

Nesta disciplina, **Peça** é o item individual do Portfólio, e só isso. Os itens da coleção do Projeto Autoral se chamam **artefatos**. As skills seguem essa distinção, e vale seguir também nas conversas de vocês, para ninguém se confundir na hora da entrega.
