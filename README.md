# - FuncoesJs 
<br>

### Atividade disciplinar de Linguagem Script
 <br>
 
 ## Assunto: Funções de declaração, expressão e arrow.
 <br>
 
 No JavaScript, uma função é um bloco de código que realiza uma tarefa específica e pode ser reutilizada. É uma das ferramentas mais importantes para escrever código organizado, legível e modular. Uma função é, essencialmente, um procedimento que executa uma tarefa ou calcula um valor onde  utilizar comandos com  Bloco de Código, trabalhando com  Reutilização de código, deixando os códigos mais Organizado facilitando na criação de Objetos de Primeira Classe.
 <br> 
 <br>
 
```javascript
var square = function (numero) {
  return numero * numero; 
};
var x = square(4);   // x recebe o valor 16
```
<br>

**numero:** é o parâmetro, dentro do parânteses é como a função recebe um valor quando for chamada.
<br>

**Return:** ele retorna o valor multiplicando.
<br>

**square(4):**  é a chamada onde O número 4 é o argumento e o valor real passa para o parâmetro numero.
<br>
<br>


# function declaration (declaração de função)
<br>

Ela define uma função com os parâmetros específicos para uma função criada com uma declaração tem toda as propriedades, métodos e comportamento dos objetos na **function**, podendo ser chamada em qualquer parte do código.
<br>

##  Vantagem
<br>
As funções declaradas possui hoísting, ou seja são movida para o topo esboço em que foram declaradas, sendo possivel chamar a função antes dela ser declarada, além disso são fáceis de serem indentificadas e debugadas, por terem nomes para referenciá-las, ela é uma forma simples e eficiente de declarar funções em javascript.
<br>

##  Desvantagem
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
<br>

# expression function (expressão de função)
<br>

 A expressão tem semelhança a função de declaração, tendo quase a mesma sintaxe. A principal diferença entre eles é o nome da função, que pode ser onitido em expressões para criar funções anônimas, essa função não são içadas, ao contrário da declarada, você não pode usar expressões de funções antes mesmo de criá-las.
 <br>
 
 ##  Vantagens
 
 <br>
 
- **anônimas:** permitem criar funções sem nome, em contexto onde ela não precisa ter um nome definido.
<br>

- **Uso em expressões:** podem ser utilizadas dentro de outras expressões como em callbacks de funções array.
<br>

- **Versabilidade:** elas podem ser definidas como variáveis e são frequentemente utilizadas em situações que exigem funções que são passadas como argumentos ou retornadas por outras funções.

<br>

##  Desvantagens

<br>

- **Ausência de hoisting:** As expressões de função, as aunônimas não são "içadas" como a declarada. isso significa que você precisa declarar a função antes de usá-la no código, senão o javascript lançará um erro.

  <br>

- **Legibilidade e manutenção:** as funções anônimos da expressão podem tornar o código mais difícil de ler e de manter, também quando tem funções complexas ou recursivas.

<br>

- **Complecidade de debugging:** debugar expressões anônimas podem ser mais difícil , pois as funções não tem nome e podem ser difícil de indentificar em chamadas complexas.

<br>

Em resumo, as expressões de funções são  úteis em situações específicas, mas é importante está ciente das suas desvantagens para tomar decisões informados sobre qual tipo de função usar na decisão de seus projetos.

<br>

### Exemplos de códigos: 

<br>

```javascript
const getRectArea = function(width,height){
      return width * height;
}
console.log(3,4);
```

```javascript
const foo = function*(){
yield "a";
yield "b";
yield "c";
}
let str = '';
for (const val of foo()){
str = str + val;
}
console.log(str);
```

```javascript
let sayhi = function(){
alert("hello");
};
```
<br>

# Function Arrow (função de seta)
<br>

Uma expressão de função de seta, é uma alternativa compactar as expressões de função tradicionais, de forma simples, ela otimiza a escrita do seu código, deixando mais limpo, aumentando a legibilidade por utilizar comandos de "=>" facilitando na criação de novas funcionalidade.
<br>

## Vantagens 
<br>
 Na função de seta ela permite escrever uma sintaxe de função mais curta, por serem menos verbosas (não precisando escrever muitas linhas de código) do que as funções tradicionais, As funções de seta oferecem uma forma mais eficiente e legível de escrever funções em JavaScript, especialmente para situações que exigem funções de uma linha ou que lidam com callbacks e no valor do "this", ela é  definida a partir das funções onde foram definidas, não sendo necessário usar o método blint().
<br>

## Desvantagens
<br>

A principal falta de contexto do "this" próprio, isso leva a problemas se precisar se referenciar o contexto da própria arrow function, não podendo ser usado como construtores e também não possuem argumentos, sintaxe mais curta pode dificultar a leitura.
<br>

### Exemplos de código:
<br>

```javascript
let age = prompt("What is your age?", 18);

let welcome = (age < 18) ?
  () => alert('Hello!') :
  () => alert("Greetings!");

welcome();
```
<br>

```javascript
const dobrar = (numero) => numero * 2;
```
<br>

```javascript
const calcularMedia = (notas) => {
 const soma = notas.reduce((total, nota) => total + nota, 0);
 return soma / notas.length;
};
```
<br>
