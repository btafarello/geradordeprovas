# Gerador de Provas Dissertativas — Colégio Criarte

Ferramenta web estática (HTML, CSS e JavaScript em arquivo único) desenvolvida para padronizar as avaliações dissertativas do **Colégio Criarte** sem exigir formatação manual por parte dos professores.

## Estrutura do repositório

| Arquivo | Função |
| :--- | :--- |
| `index.md` | Página inicial renderizada pelo GitHub Pages com instruções rápidas e link direto para o gerador. |
| `gerador_provas_dissertativas.html` | Aplicação interativa completa (formulário guiado + prévia A4 ao vivo + impressão em PDF). |
| `README.md` | Documentação técnica e guia de publicação para a coordenação pedagógica. |

## Recursos incluídos

- **Capa oficial do Colégio Criarte:** bloco de logotipos (Colégio Criarte, Cambridge University Press, Academia Washington e Sistema de Ensino Anglo), banner superior dinâmico por segmento e cabeçalho em caixas arredondadas (*Avaliação de Ciclo*, *Data*, *Período*, *Disciplina*, *Professor*, *Valor*, *Série*, *Turma*, *RM*, *Nome*, *Nº* e *Nota*).
- **Seleção inteligente por segmento:** ao escolher *Fundamental I*, *Fundamental II* ou *Ensino Médio*, as opções de séries/anos e disciplinas se ajustam automaticamente.
- **Quadro de Conteúdo e Instruções oficiais:** lista de conteúdos gerada linha a linha com marcadores (`➤`) e bloco com as 9 instruções padrão da escola na página 1.
- **Caderno de questões padronizado:** inserção de contextualização opcional, atalhos de verbos de comando, controle deslizante de linhas pautadas por questão e soma automática de pontuação.
- **Versão do Aluno e Gabarito do Professor:** alternância em um clique entre as pautas em branco e a expectativa de resposta de cada questão.
- **Impressão limpa em A4:** folha de estilo dedicada (`@media print`) que oculta o formulário e separa a capa (página 1) do caderno de questões (página 2 em diante).
- **Zero servidor e salvamento local:** roda 100% no navegador com salvamento automático de rascunho via `localStorage`.

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub (por exemplo, `gerador-provas-criarte`) e envie os arquivos `index.md`, `README.md` e `gerador_provas_dissertativas.html` para a raiz da branch `main`.
2. No repositório, acesse **Settings** → **Pages** (no menu lateral esquerdo).
3. Em **Build and deployment**, selecione **Deploy from a branch**.
4. Em **Branch**, escolha `main` e a pasta `/ (root)`, depois clique em **Save**.
5. Aguarde cerca de 1 a 2 minutos até o GitHub gerar o endereço público no formato:

```text
https://[SEU-USUARIO].github.io/[NOME-DO-REPOSITORIO]/
```

> **Dica:** se você preferir que o link principal abra o gerador diretamente (sem passar pela página inicial `index.md`), basta renomear `gerador_provas_dissertativas.html` para `index.html` na raiz do repositório.

## Uso local (offline)

Também é possível utilizar a ferramenta sem internet (exceto o carregamento inicial dos ícones/estilos): basta baixar o arquivo `gerador_provas_dissertativas.html` e abri-lo com duplo clique em qualquer navegador moderno.
