# Javascript
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
        let variávelB = "Hello " + variávelA
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