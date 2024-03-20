# Javascript

## Variáveis
As variáveis são usadas para armazenar dados. Existem três tipos no Javascript:
- Var: utilizada quando necessitar de variável global ou uma variável que possa ser redeclarável;
```javascript
var nome = "Ana";
console.log(nome)
```
- Let: utilizada para loops e não é redeclarável, mas pode ser atualizada;
```javascript
let num = 22;

if (num > 21){
    let mensagem = "Número maior que 21";
    console.log(mensagem)
}
```
- Const: utilizada na maioria dos casos, menos quando precisar redeclarar ou atualizar uma variável.
```javascript
const mês = 10;
console.log(mês)
```

## Escopo
Escopo é a região em que as variáveis são acessíveis. Existem os globais, de bloco e de função.
- Global: quando as variáveis são declaradas fora de uma função, pois podem ser usadas em qualquer parte do código;
```javascript
var variável = "global";

function funçãoGlobal(){
    console.log(variável) // variável é global, então é acessível aqui
    }
```
- Bloco: quando as variáveis são declaradas dentro de uma condição, como: condicional if, loop for, loop while. No escopo de bloco, as variáveis **let** e **const** só serão acessadas dentro de condições. Já com o **var**, o escopo poderá ser acessado em qualquer parte do código.
```javascript
function funçãoBloco(variávelA) {
    if (true) {
        var variávelB = "Hello " + variávelA
    };
    return variávelB;
}
funçãoBloco("World");

console.log(variávelA) // A variávelA foi definida dentro da função, portanto não é acessada
```
- Função: quando as variáveis são declaradas dentro de uma função, as **locais**, e só são acessíveis dentro dela.
```javascript
function funçãoFunção(){
   if(true) {
     let num = 5
   };
   console.log(num);
 }

 funçãoFunção() // A variável num está sendo chamada fora da função, portanto, retornará que ela não está definida
 ```

## Tipos de dados
#### Dados Primitivos
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
- Undefined: designado quando uma variável vazia é criada;
```javascript
var nome;
console.log(nome)
```
- Null: nada ou objeto vazio; 
```javascript
var nome = null;
console.log(nome)
```

#### Objeto