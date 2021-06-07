# REDUX-Angular-NGRX

## ideias principais:
* todos os dados da aplicação se encontra em uma estrutura definida.
* todas informações se encontra em um unico lugar, chamado STORE.
* o STORE nunca é modificado de forma direta.
* interações do usuario no codigo dispara ações que descrevem o que aconteceu.
* o valor atual das informações da aplicação se chama estado - STATE.
* um novo estado é criado, com base na combinação do estado antigo e uma ação por uma função chamada REDUCER.

# ACTION - REDUCER - STATE - STORE
## ACTION
* é a unica fonte de informação enviada pelo usuário ou pelas interações do programa
* em geral, pretende-se que as ações sejam o mais simples possível
* uma ACTION tem unicamente 2 propriedades (type e payload).

## REDUCER
* é uma função que recebe apenas 2 argumentos.
* e sempre retonar um estado.
* estado velho -> ação

## STATE
* o state é somente leitura.
* nunca é alterado de forma direta.
* existem funções proibidas de js ( Push e manipulação direta do objeto).

## STORE
* contem o estado atual da aplicação
* permite a leitura atual do estado via: getState()
* permite criar um novo estado utilizando: dispatch(ACTION)
* permite notificar as mudanças de estado via subscribe()
