---
name: gerar-charters-testes-exploratorios
description: Gerar, revisar e organizar charters de testes exploratorios para a disciplina Projeto Orientado em Computacao, seguindo o padrao da professora Debora/UFS. Use quando Codex precisar criar charters CHT, areas de concentracao com checkboxes, issues de bugs e melhorias no GitHub, referencias cruzadas entre Charter e Bug/Melhoria, charters subsequentes CHT1.1, ou planos de sessao baseados em heuristicas de teste exploratorio.
---

# Gerar Charters Testes Exploratorios

## Fluxo Principal

Use esta skill para transformar escopo, mapa conceitual, funcionalidades, telas, requisitos ou repositorios GitHub em charters e issues no formato esperado pela disciplina.

1. Identificar o item do escopo/funcao que sera explorado e atribuir um identificador `CHTn`.
2. Criar um charter por item relevante do mapa conceitual/escopo, com responsavel de teste quando conhecido.
3. Escrever o charter como issue GitHub com label `Charter`.
4. Usar `- [ ]` em cada item de `Areas de concentracao`; isso deve virar tarefa/checklist dentro da issue.
5. Planejar uma sessao curta e focada, normalmente 60 minutos, com testador, data, hora de inicio, setup e notas.
6. Durante a exploracao, criar uma issue separada para cada bug ou melhoria, sempre referenciando o charter que encontrou o problema.
7. Fazer referencia cruzada: a issue do bug/melhoria aponta para o charter, e o charter lista o bug/melhoria com o numero da issue.
8. Ao encerrar a sessao, atualizar o charter com tempo real usado, bugs, melhorias, verificacoes pendentes e notas, depois fechar a issue do charter.

Leia `references/padroes-da-disciplina.md` quando precisar aplicar regras de GitHub, labels, numeracao, fechamento e relacao com mapa conceitual.
Leia `references/heuristicas.md` quando precisar escolher boas areas de concentracao ou ataques de dados.
Leia `references/templates-github.md` quando precisar devolver corpos prontos de issues para Charter, Bug ou Melhoria.

## Regras De Saida

Preserve os identificadores da disciplina:

- Charters: `CHT1`, `CHT2`, `CHT3`.
- Charters subsequentes: `CHT1.1`, `CHT1.2`.
- Bugs: `CHT1-Bug1`, `CHT1-Bug2`.
- Melhorias: `CHT1-Melhoria1`, `CHT1-Melhoria2`.

Ao criar charters, seja especifico o suficiente para guiar a sessao, mas nao tente transformar o charter em roteiro fechado. Em testes exploratorios, o design completo evolui durante a execucao.

Ao criar bugs ou melhorias, inclua passos, resultado obtido, resultado esperado/proposto, evidencias e referencia ao charter. Nao agrupe bugs diferentes na mesma issue.

Quando alguma area de concentracao nao couber no tempo da sessao, proponha charters subsequentes e registre isso em `Notas`.

## Qualidade Esperada

Use heuristicas para evitar charters superficiais. Priorize riscos de:

- adequacao funcional;
- obrigatoriedade e validacao de campos;
- datas, numeros, strings e limites;
- permissoes/roles;
- consistencia entre estados e dados;
- CRUD;
- navegacao web, refresh, voltar, URLs e multiplas sessoes;
- usabilidade, texto, feedback e acessibilidade basica;
- multiusuario, sequencias e interrupcoes quando fizer sentido.

Nunca invente numeros de issues GitHub. Se o numero ainda nao existir, use um marcador como `#TODO` ou diga que deve ser preenchido apos criar a issue.
