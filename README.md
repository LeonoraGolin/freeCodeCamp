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


