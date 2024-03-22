# Javascript
## Tipos de dados
### Dados Primitivos
Os principais dados primitivos no Javascript são: boolean, number, string, undefined, null.

- Boolean: dado lógico que pode assumir valor de **true** ou **false**;
```javascript
var a = true;

if(a === true){
    console.log("a tem valor de true");
}
```
- Number: dado numérico, sendo este decimal ou não;
```javascript
const num = 0.5;
console.log(num);
```
- String: são usadas para representar dados textuais. Cada elemento representa um índice, que começa no 0. As strings são imutáveis;
```javascript
const dia = "O dia está ensolarado";
console.log(dia)
```
- Undefined: designado quando uma variável vazia é criada, não é definida;
```javascript
var nome;
console.log(nome)
```
- Null: nada ou objeto vazio; 
```javascript
var nome = null;
console.log(nome)
```

### Objeto
Um objeto é uma coleção de pares de chave-valor, onde cada chave é uma string e cada valor pode ser de qualquer tipo de dado, incluindo outros objetos. 
```javascript
var pessoa = {
    nome: "Maria",
    idade: 20,
    casado: false,
    endereço: {
        rua: "Rua Maravilha",
        cidade: "Alegria",
        país: "Brasil"
    }}
```
Aqui, **pessoa** é um **objeto** com **chaves**, propriedades, como nome e cada chave tem seu **valor** (Maria, no caso do nome). A chave endereço é um outro objeto que também possui chaves e valores.

Existem duas formas de acessar objetos:
```javascript
console.log(pessoa.nome); // usando objeto.propriedade
console.log(pessoa['idade']); // usando objeto['propriedade']
```

### Array
Em JavaScript, um array é uma estrutura de dados que permite armazenar uma coleção ordenada de elementos. Os elementos podem ser de qualquer tipo de dado. Os arrays são dinâmicos, ou seja, podem crescer ou diminuir de tamanho durante a execução do programa.
```javascript
var frutas = ['maçã', 'banana', 'laranja', 'pera'];
```
Cada elemento está associado a um índice numérico, começando em 0 para o primeiro elemento.
```javascript
console.log(frutas[0]); // Saída: "maçã"
```
É possível modificar os elementos de um array a partir do índice:
```javascript
frutas[1] = 'morango'; // Modifica o segundo elemento para "morango"
```
Existem muitos métodos para manipulção de arrays, sendo eles: length(), push(), pop(), shift(), unshift() e splice()