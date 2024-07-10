# Deletando e editando propriedades

Em um sistema, muitas vezes será necessário deletar ou editar uma informação guardada em objetos.

A linguagem JavaScript nos permite editar e deletar propriedades de objetos já criados.

Tendo o exemplo utilizado em aula como base:

```
const listaDeCompras = {
    compra1: "Arroz",
    compra2: "Feijão",
    compra3: "Biscoito"
}
```

## Deletando chave e valor de objetos

Vamos supor que eu queira deletar a chave `compra2` e o seu valor `”Feijão”`, do objeto `listaDeCompras`:

```
delete listaDeCompras.compra2   
console.log(listaDeCompras) 
```

O console irá retornar: `{compra1: 'Arroz', compra3: 'Biscoito'}`

## Editando o valor de uma chave

E se for preciso apenas editar o valor de alguma chave? Por exemplo, alterar o valor da chave `compra3`, que é `”Biscoito”`, para `”Bolacha”`.

É possível da seguinte forma:

```
listaDeCompras.compra3 = "Bolacha"

console.log(listaDeCompras.compra3)
```

O console irá retornar: `Bolacha`

Diferente de deletar que é necessário o comando `delete`, para **editar o valor de uma chave** é preciso apenas passar **o nome do objeto + chave, seguido de sinal de igual + o novo valor que deseja substituir**.

### E se eu quiser deletar um objeto por completo do sistema ou alterar o seu nome?

Nesse caso, não é permitido alterar o nome de um objeto, ou deletá-lo, **uma vez já declarado**. Uma alternativa seria criar um clone do objeto, copiando as propriedades que ele guarda. Dessa forma, serão criados dois objetos no sistema. Você pode aprender na prática como clonar objetos no vídeo a seguir! :)

#### [Voltar ao Readme principal](../README.md)