# O que é o filter no JavaScript e no Python?

## JavaScript

Em JavaScript, o filter é uma função de array que permite filtrar elementos com base em uma condição definida. Ele cria um novo array contendo apenas os elementos que atendem à condição especificada. A sintaxe básica do filter é a seguinte:

```javascript
array.filter(function(valor, índice, arrayOriginal) {
    // Condição de filtro
});
```

Aqui está um exemplo de como usar o filter para filtrar apenas os números pares de uma matriz:

```javascript
const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const numerosPares = numeros.filter(function(numero) {
    return numero % 2 === 0;
});

console.log(numerosPares); // Output: [2, 4, 6, 8, 10]

```

## Python
Em Python, o filter é uma função que permite filtrar elementos com base em uma função de teste. Ele cria um iterador que retorna apenas os elementos que passam no teste especificado pela função. A sintaxe básica do filter é a seguinte:

```python
filter(funcao_de_teste, iteravel)
```

Aqui está um exemplo de como usar o filter para filtrar apenas os números pares de uma lista:
```python
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

numeros_pares = list(filter(lambda numero: numero % 2 == 0, numeros))

print(numeros_pares) # Output: [2, 4, 6, 8, 10]
```

Neste exemplo, usamos a função lambda para definir a função de teste que verifica se um número é par ou não. Em seguida, passamos essa função e a lista de números como argumentos para o filter. Por fim, convertemos o resultado do filtro em uma lista usando a função list().
