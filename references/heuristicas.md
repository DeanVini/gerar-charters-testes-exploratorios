# Heuristicas Para Gerar Areas De Concentracao

Use estas heuristicas para criar missoes de teste, checklists de `Areas de concentracao` e ideias de dados.

## Ataques De Dados

Datas e horas:

- dias invalidos, como 30/02 e 31/09;
- 29/02 em ano nao bissexto;
- formatos diferentes, como `05/06/2001`, `06-05-01`, `6/5/2001 12:34`;
- data inicial maior que data final;
- mudanca de fuso horario, horario de verao, relogio adiantado/atrasado.

Numeros:

- `0`, `1`, valores negativos;
- limites como `32768`, `65536`, `2147483648`, `4294967296`;
- decimais, notacao cientifica, numeros com virgula, formato europeu;
- usar esses valores em calculos e validacoes.

Strings:

- vazio, espaco unico, multiplos espacos, espacos no inicio/fim;
- textos longos: 255, 256, 257, 1000, 1024, 2000 caracteres;
- caracteres acentuados, asiaticos e cirilicos;
- delimitadores e caracteres especiais como `"`, `'`, `|`, `/`, `\`, `,`, `;`, `:`, `&`, `<`, `>`, `*`, `?`, tab;
- tentativas de SQL injection e HTML/JavaScript injection.

Arquivos/caminhos:

- nomes longos, caracteres especiais, arquivo inexistente, arquivo ja existente;
- sem espaco, espaco minimo, protegido contra escrita, bloqueado, remoto, corrompido.

## Web E Navegacao

- Voltar no navegador e observar mensagens expiradas ou transacoes duplicadas.
- Refresh apos enviar formulario.
- Favoritar URL e abrir logado/deslogado.
- Alterar/remover parametros da URL.
- Abrir multiplas instancias do navegador.
- Desativar JavaScript, cookies ou elevar configuracao de seguranca.
- Redimensionar janela e mudar tamanho da fonte.
- Verificar tamanho maximo em inputs e textos com mais de 5000 caracteres em textareas.

## Heuristicas Gerais

- Analise de variaveis: identificar tudo que pode mudar.
- Pontos de toque: interfaces publicas/privadas que permitem provocar, monitorar e verificar.
- Limites: quase no limite, exatamente no limite, alem do limite.
- Goldilocks: grande demais, pequeno demais, adequado.
- CRUD: criar, ler, atualizar, deletar.
- Seguir os dados: inserir, buscar, relatar, exportar, importar, atualizar e visualizar.
- Configuracoes: resolucao, rede, latencia, memoria, disco e perifericos.
- Interrupcoes: logout, desligar, reiniciar, matar processo, desconectar, hibernar, timeout, cancelar.
- Escassez: CPU, memoria, rede ou disco no maximo.
- Posicao: inicio, meio e fim.
- Selecao: alguns, nenhum, todos.
- Contagem: zero, um, muitos.
- Multiusuario: criacao, atualizacao ou delecao simultanea por duas contas ou mesma conta em duas sessoes.
- Dependencias: objetos com relacao `tem um/tem muitos`, aplicando CRUD, contagem, posicao e selecao.
- Restricoes: obrigatorios vazios, combinacoes invalidas, duplicidade.
- Metodo de entrada: digitar, copiar/colar, importar, arrastar/soltar, GUI vs API.
- Sequencias: mudar ordem, desfazer/refazer, inverter, combinar, simultaneo.
- Ordenacao: alfabetica vs numerica e multiplas paginas.
- Estados: identificar estados, eventos e transicoes.
- Usuarios e cenarios: casos de uso, personas e perfis extremos.

## Sabedoria De Teste

Um teste e um experimento para revelar informacao ou responder uma pergunta sobre o software. Varie sequencias, configuracoes e dados para aumentar a chance de encontrar problemas. Bugs tendem a se agrupar; uma descoberta pode indicar uma area de risco maior.
