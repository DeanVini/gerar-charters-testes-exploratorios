# Templates GitHub

Use os templates abaixo como base. Ajuste os campos ao contexto real e remova secoes sem informacao.

## Issue De Charter

```markdown
## Identificacao

CHTn: <nome da funcionalidade/area>

## Objetivo

<missao da sessao exploratoria>

## Areas de concentracao

- [ ] <risco/cenario/heuristica 1>
- [ ] <risco/cenario/heuristica 2>
- [ ] <risco/cenario/heuristica 3>

## Setup (pre-condicoes)

- <usuarios, roles, massa de dados, ambiente, navegador/dispositivo>
- <estado inicial necessario>

## Testador(a)

<nome>

## Data da sessao

<dd/mm/aaaa>

## Hora de inicio

<hh:mm>

## Duracao planejada

<ex.: 60 minutos>

## Verificar

- <questoes que precisam de confirmacao para decidir se sao bugs>

## Bugs

- <CHTn-Bug1 #TODO>

## Melhoria identificada

- <CHTn-Melhoria1 #TODO>

## Notas

- <areas de risco, oportunidades para novos charters, limitacoes da sessao>
- Tempo real utilizado: <preencher ao fechar>
```

## Issue De Bug

```markdown
## Identificacao

CHTn-Bugm: <titulo curto do problema>

## Charter relacionado

Encontrado durante #<numero-da-issue-do-charter> (`CHTn`).

## Ambiente

- Versao/plataforma:
- Navegador/dispositivo:
- Usuario/role:

## Passos para reproduzir

1. <passo>
2. <passo>
3. <passo>

## Resultado obtido

<o que aconteceu>

## Resultado esperado

<o que deveria acontecer>

## Evidencias

<screenshots, video, logs, dados usados>

## Observacoes

<impacto, frequencia, hipoteses, regra de negocio pendente>
```

## Issue De Melhoria

```markdown
## Identificacao

CHTn-Melhoriam: <titulo curto da melhoria>

## Charter relacionado

Identificada durante #<numero-da-issue-do-charter> (`CHTn`).

## Comportamento atual

<como funciona hoje>

## Proposta

<novo comportamento sugerido>

## Justificativa

<beneficio esperado, problema de usabilidade, clareza, eficiencia ou consistencia>

## Evidencias/cenario

<prints, passos, exemplos de uso, comparacao>

## Observacoes

<restricoes, alternativas, perguntas para a equipe>
```

## Atualizacao No Charter Apos Abrir Bugs/Melhorias

```markdown
## Bugs

- CHTn-Bug1 #123
- CHTn-Bug2 #124

## Melhoria identificada

- CHTn-Melhoria1 #125
```
