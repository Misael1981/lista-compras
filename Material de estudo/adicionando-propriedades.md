# Adicionando propriedades

A linguagem JavaScript é do tipo orientada a objetos, isso significa que, objetos são a parte central dessa linguagem, dessa forma, é importante entender como manipular as informações que um objeto guarda.

Já os objetos nos permitem trazer para o mundo da programação elementos do mundo real, transformando-os em dados, e, a partir disso, ser possível trabalhar com esses dados.

## Estrutura de um objeto literal

Criamos objetos literais e descobrimos como é formada sua estrutura:

```
const cliente = { nome: ‘Mariana’ }

//variável nomeDoObjeto = { chave: valor}
```

O objeto literal no JavaScript é formado por uma coleção de propriedades. Uma propriedade é formada pelo conjunto chave + seu valor, no exemplo acima temos a propriedade `nome`, que é o conjunto da chave `nome`+ valor `’Mariana’`.

## Adicionando propriedades em um objeto

Vamos supor que seja necessário adicionar propriedades em um objeto. Existem diferentes notações que nos possibilitam chegar a esse objetivo, a mais comum é a de ponto.

Vamos conferir nesse exemplo:

```
const cliente = { nome: ‘Mariana’ }

cliente.idade = 35

console.log(cliente)
```

O console irá retonar:

```
{
   nome: 'Mariana', 
   idade: 35
}
```

É possível conferir que foi adicionado a chave idade, com valor 35, que anteriormente não existia.

No exemplo acima foi utilizado a notação de ponto, e existe também a notação de colchetes.

Vamos conferir como utilizar a notação de colchetes para adicionar propriedades em um objeto:

```
cliente = {
   nome: 'Mariana', 
   idade: 35
}

cliente['genero'] = 'Feminino'

console.log(cliente)
```

O console irá retonar:

```
{
   nome: 'Mariana', 
   idade: 35, 
   genero: 'Feminino'
}
```

Note que a chave foi passada entre aspas, ou seja, no formato de string. Com isso, podemos chegar à conclusão que chaves de objetos também podem ser dados do tipo string. Como no exemplo abaixo:

```
cliente = {
   'nome': 'Mariana', 
   'idade': 35,
   'sexo': 'Feminino'
 }
```

#### [Readme principal](../README.md)