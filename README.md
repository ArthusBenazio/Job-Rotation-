# Job-Rotation
## Desafio Job Rotation

### Resposta questão 1:

const indice = 13
let soma = 0
let k = 0

while(k < indice) {
k = k + 1
soma = soma + k
}

console.log(soma)

resultado 91

### Resposta questão 2:

let num = prompt("Digite um número:");
num = parseInt(num);

let fib = [0, 1];
while (fib[fib.length - 1] < num) {
    fib.push(fib[fib.length - 1] + fib[fib.length - 2]);
}

if (fib.includes(num)) {
    console.log(`O número ${num} pertence à sequência de Fibonacci.`);
} else {
    console.log(`O número ${num} não pertence à sequência de Fibonacci.`);
}

### Resposta questão 3:

a) 1, 3, 5, 7, "9"

b) 2, 4, 8, 16, 32, 64, "128"

c) 0, 1, 4, 9, 16, 25, 36, ____

d) 4, 16, 36, 64, ____

e) 1, 1, 2, 3, 5, 8, "13"

f) 2,10, 12, 16, 17, 18, 19, ____

### Resposta questão 4:

Quandos eles se cruzarem ambos vão estar a mesma distância de Ribeirão Preto.

### Resposta questão 5:

let str = "Hello, world!";

let arr = str.split("");

for (let i = 0; i < Math.floor(arr.length / 2); i++) {
  let temp = arr[i];
  arr[i] = arr[arr.length - 1 - i];
  arr[arr.length - 1 - i] = temp;
}

let invertedStr = arr.join("");

console.log(invertedStr);
