#algoritmos básicos

#função para converter celsius em fahrenheit
function convertToF(celsius) {
  let fahrenheit = (celsius*9/5)+32;  
  return fahrenheit;
}
convertToF(30);

#função para inverter uma string
function reverseString(str) {
  let reverse = "";  
  for (let i=str.length - 1; i >=0 ; i--) {
    reverse += (str[i]);    
  }
  return reverse;
}
reverseString("hello");

#função para fatorar um número
function factorialize(num) {
  let fat = 1;
  for (let i=1; i<=num; i++) {
    fat *= i;
  }  
  return fat;
}
factorialize(5);

#função que retorna o comprimento da palavra mais longa na frase fornecida
function maiorPalavra(str) {
  let myArr = str.split(' ');
  let max = 0;  
  for (let i=0; i<myArr.length; i++)
     if (myArr[i].length > max) {
       max = myArr[i].length;
     }  
  return max;
}
maiorPalavra("O submarino japonês foi atacado por mísseis americanos.");

#função que retorna quantidade de palavras em uma string
function quantidadePalavras(str) {
  let myArr = str.split(' ');
 return myArr.length;
}
quantidadePalavras("O submarino japonês foi atacado por mísseis americanos.");

#função quer retorna um array com os maiores números em cada sub-array 
function largestOfFour(arr) {
  let results = [];
  for (let i = 0; i < arr.length; i++) {
    let largestNumber = arr[i][0];
    for (let j = 1; j < arr[i].length; j++) {
      if (arr[i][j] > largestNumber) {
        largestNumber = arr[i][j];
      }
    }
    results[i] = largestNumber;
  }

  return results;
}
largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);
