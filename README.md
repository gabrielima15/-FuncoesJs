# - FuncoesJs 
 Assunto do Projeto da Disciplina de LS - atividade 1 tipos de funções.
 <br>
 ## Mas o que é uma função?
 <br>
 No JavaScript, uma função é um bloco de código que realiza uma tarefa específica e pode ser reutilizada. É uma das ferramentas mais importantes para escrever código organizado, legível e modular. Uma função é, essencialmente, um procedimento que executa uma tarefa ou calcula um valor onde  utilizar comandos com  Bloco de Código, trabalhando com  Reutilização de código, deixando os códigos mais Organizado facilitando na criação de Objetos de Primeira Classe.
 <br> <br>
 
```javascript
var square = function (numero) {
  return numero * numero; 
};
var x = square(4);   // x recebe o valor 16
```
<br>

# function declaration (declaração de função)
<br>

Ela define uma função com os parâmetros específicos para uma função criada com uma declaração tem toda as propriedades, métodos e comportamento dos objetos na **function**, podendo ser chamada em qualquer parte do código.
<br>

## ° Vantagem
<br>
As funções declaradas possui hoísting, ou seja são movida para o topo esboço em que foram declaradas, sendo possivel chamar a função antes dela ser declarada, além disso são fáceis de serem indentificadas e debugadas, por terem nomes para referenciá-las, ela é uma forma simples e eficiente de declarar funções em javascript.
<br>

## ° Desvantagem
<br>
Em contra partida devdo ao hoísting, declarar uma função com o mesmo nome em diferentes partes do código pode resultar na sobreescrita da função inicial. álem de possuir menor controle  de  escopo, o que pode dificultar a modulalização do código.
<br>

### Exemplos em código:
<br>

```javascript
function saudacao(){
console.log("olá!");
}
saudacao()
```
<br>

```javascript
function soma(a,b){
return a + b;
}
let resultado = soma(3,4);
console.log(resultado);
```
<br>

```javascript
function script(){
   var hello_world = "hello world!";
   return hello_world;
}
script();
```
