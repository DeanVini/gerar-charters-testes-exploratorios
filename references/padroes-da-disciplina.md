# Padroes Da Disciplina

## Organizacao No Mapa Conceitual

- Para cada item definido no escopo do projeto ou mapa conceitual, criar os respectivos charters no mapa e no GitHub.
- Identificar os responsaveis pelos testes em cada item do escopo quando a informacao existir.
- Atualizar o mapa conceitual quando surgirem charters subsequentes, como `CHT1.1` ou `CHT2.1`.

## Repositorio GitHub

- Se a versao web estiver sendo testada, criar charters, bugs e melhorias no repositorio web.
- Se a versao mobile estiver sendo testada, criar no repositorio mobile.
- Se o projeto estiver separado em front-end e back-end, registrar charters e bugs encontrados pela equipe de testes no repositorio front-end. Quando o bug for de back-end, a equipe autora do projeto deve abrir a issue correspondente no repositorio back-end.
- Membros da equipe de testes usam role `Triage`.

## Issues De Charter

- Criar cada charter como issue GitHub.
- Usar identificacao `CHT1`, `CHT2`, etc.
- Usar `CHT1.1`, `CHT1.2` quando o charter for consequencia de outro.
- Aplicar label `Charter`.
- Em `Areas de concentracao`, escrever cada item como `- [ ]` para virar tarefa na issue.
- Ao termino da sessao, fechar a issue de Charter e documentar o tempo realmente utilizado.

## Bugs

- Ao encontrar um bug durante a exploracao, criar uma issue GitHub separada.
- Aplicar label `Bug`.
- Usar identificacao `CHT1-Bug1`, `CHT1-Bug2`.
- Referenciar o charter responsavel pela identificacao.
- Incluir tudo que for necessario para explicar o bug: screenshots, passos para reproducao, gravacao, dados usados, ambiente, resultado obtido e resultado esperado.
- Fazer referencia cruzada: o bug aponta para o charter e o charter lista o bug com o numero da issue.

## Melhorias

- Ao encontrar uma melhoria durante a exploracao, criar uma issue GitHub separada.
- Aplicar label `Melhoria`.
- Usar identificacao `CHT1-Melhoria1`, `CHT1-Melhoria2`.
- Referenciar o charter responsavel pela identificacao.
- Incluir o comportamento atual, proposta de comportamento, justificativa, evidencias e passos/cenario quando houver.
- Fazer referencia cruzada com o charter.

## Charters Subsequentes

Abrir charters subsequentes quando:

- algum item de `Areas de concentracao` nao for explorado ate o fim da sessao;
- surgir uma nova oportunidade de exploracao sem tempo para analisar;
- a oportunidade fugir demais da missao da sessao atual.

Ao criar o charter subsequente antes da execucao, colocar apenas o necessario para lembrar o objetivo. Completar o charter quando a sessao for realmente executada.

## Fechamento E Validacao

- Fechar a issue de Charter ao fim da sessao, com tempo real utilizado.
- Issues de bug/melhoria so devem ser fechadas pelo criador da issue, apos validar a correcao ou implementacao feita pela equipe autora do projeto.
- Se algo parecer bug mas depender de regra de negocio, registrar em `Verificar` antes de abrir ou concluir a issue definitiva.
