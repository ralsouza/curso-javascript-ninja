# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function(x,y) {
  resultado = x + y;
  return resultado;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var x = soma(3,2) + 5;

// Qual o valor atualizado dessa variável?
10

// Declare uma nova variável, sem valor.
var y;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function retorna_valor(valor) {
  y = valor;
  return 'O valor da variável agora é: ' + valor;
}

// Invoque a função criada acima.
retorna_valor(3)

// Qual o retorno da função? (Use comentários de bloco).
/*
  O valor da variável agora é: 3
*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function calc( x, y, z ) {
  if ( x === undefined || y === undefined || z === undefined) {
    return 'Preecha todos os valores corretamente!';
  } else {
    resultado = ( x * y * z ) + 2;
  }
 return resultado;
}

// Invoque a função criada acima, passando só dois números como argumento.
calc(2, 3);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// 'Preencha todos os valores corretamente!'

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
calc(2, 3, 4);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// 26

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function calc2 ( a, b, c) {
  if ( a !== undefined && b === undefined && c === undefined ) {
    return 'O valor do parâmetro a é: ' + a;
    // Se o a não for preenchido, com certeza b e c também não serão.
    // Logo não é necessário testar se b e c foram preenchidos.
    } else if ( a !== undefined && b !== undefined && c === undefined ) {
      soma1 = a + b;
      return 'A soma de a com b é: ' + soma1;
    } else if ( a !== undefined && b === undefined && c !== undefined ) {
      soma2 = a + c;
      return 'A soma de a com c é: ' + soma2;
    } else if ( a === undefined && b !== undefined && c !== undefined ) {
      soma3 = b + c;
      return 'A soma de b com c é: ' + soma3;
    } else if ( a !== undefined && b !== undefined && c !== undefined ) {
      soma4 = ( a + b ) / c;
      return 'O resultado do cálculo dos 3 parâmetros é: ' + soma4;
    } else if ( a === undefined && b === undefined && c === undefined ) {
      return false;
    } else {
      return null;
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
// calc2();
// false

// calc2(2);
// 'O valor do parâmetro a é: 2'

// calc2(2, 4);
// 'A soma de a com b é: 6'

// calc2( 2, 4, 5);

```
