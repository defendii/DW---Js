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