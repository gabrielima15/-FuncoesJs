# -FuncoesJs
Este é um Projeto sobre Função na Disciplina de Linguagem de Script cuja linguagem utilizada é a linguagem JavaScript. Nesse Readme.md haverá os tipos, definições e exemplos de função em Js.
<br>
# **function declaration (função declaração)**
<br>
 A função declaração define uma função com os parâmetros específicos, **uma função criada com a declaração tem todas as propriedades, métodos e comportamento dos objetos na função**, podendo ser chamada em qualquer parte do código, a sintaxe será da seguinte forma: <br>

```javascript
function nome(parâmetro1,parâmetro2,parâmetro3){
//--> código a ser executado(statements);
}
```
-**nome:** define  o nome da função;
<br>
-**parametro:** cria um argumento para ser passado para a função, tendo o seu limite de até 255 argumentos;
<br>
-**declarações:** da as instruções que compõe o corpo da função.
<br>
<br>
 por padrão as funções retornam em **UNDERFINED**.
 <br>
 <br>
 **UNDERFINED:** ele é um valor primitivo atribuído automaticamente pelo JavaScript para indicar a ausência não intencional de qualquer valor não definido.(valor vazio) 

 ## Vantagens:

 As funções declaradas dessas formas são hoisted, ou seja, são movidas para o topo do esboço em que foram declaradas, sendo possivel chamar uma função antes mesmo de sua declaração de seu código, além disso são fáceis de serem indentificados e debugada, por terem nomes para referênciá-lo, ela é  de forma simples e eficiente de declarar em JavaScript.

## Desvantagens:
Ela pode ser chamada antes  de serem definida, levando a problema de lógica e dificuldade da leitura do código levando mais tempo para corrigir. 
<br>

## Exemplos de código:

```javascript
function saudacao() {
  console.log("olá!");
}
saudacao()
```
<br>

```javascript
function soma(a,b){
return a+b;
}
var resultado = soma(3,4);
console.log(resultado);
```
<br>

```javascript
function script(){
var hello_world = "Hello World!";
return hello_world;
}
script();
```
<br>

# Function Expression(função expressão)
