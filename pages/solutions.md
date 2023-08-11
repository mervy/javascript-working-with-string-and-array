[Home](https://mervy.github.io/js-string-and-array/) | [Exercises](https://mervy.github.io/js-string-and-array/pages/exercises)

# Soluções dos exercícios

Apresente pelo menos duas soluções diferentes para cada exercício. Isso demonstrará diferentes abordagens para resolver os problemas usando JavaScript. 

Vamos lá:

**1. Crie um array de números e utilize o método `map` para elevar cada número ao quadrado.**

```javascript
// Solução 1:
const numbers = [1, 2, 3, 4, 5];
const squaredNumbers1 = numbers.map(num => num ** 2);

// Solução 2:
const squaredNumbers2 = numbers.map(function(num) {
  return num * num;
});
```

**2. Dado um array de palavras, utilize o método `filter` para retornar somente as palavras que têm mais de 5 letras.**

```javascript
// Solução 1:
const words = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
const longWords1 = words.filter(word => word.length > 5);

// Solução 2:
const longWords2 = words.filter(function(word) {
  return word.length > 5;
});
```

**3. Crie um array de números e utilize o método `reduce` para calcular a soma de todos os elementos.**

```javascript
// Solução 1:
const numbers = [1, 2, 3, 4, 5];
const sum1 = numbers.reduce((accumulator, num) => accumulator + num, 0);

// Solução 2:
const sum2 = numbers.reduce(function(accumulator, num) {
  return accumulator + num;
}, 0);
```

**4. Escreva uma função que recebe um array de números e retorna um novo array com os números pares.**

```javascript
// Solução 1:
function getEvenNumbers1(array) {
  return array.filter(num => num % 2 === 0);
}

// Solução 2:
const getEvenNumbers2 = function(array) {
  return array.filter(function(num) {
    return num % 2 === 0;
  });
};
```

**5. Dado um array de strings, utilize o método `forEach` para imprimir no console cada string em caixa alta.**

```javascript
// Solução 1:
const strings = ['apple', 'banana', 'cherry'];
strings.forEach(str => console.log(str.toUpperCase()));

// Solução 2:
strings.forEach(function(str) {
  console.log(str.toUpperCase());
});
```

**6. Crie um array de objetos, onde cada objeto representa um produto (com propriedades como nome, preço, etc.). Utilize o método `some` para verificar se existe algum produto com preço abaixo de R$ 10,00.**

```javascript
// Solução 1:
const products = [
  { name: 'apple', price: 5 },
  { name: 'banana', price: 8 },
  { name: 'cherry', price: 12 }
];
const hasCheapProduct1 = products.some(product => product.price < 10);

// Solução 2:
const hasCheapProduct2 = products.some(function(product) {
  return product.price < 10;
});
```

**7. Crie um array de números e utilize o método `every` para verificar se todos os números são positivos.**

```javascript
// Solução 1:
const numbers = [1, 2, 3, 4, 5];
const areAllPositive1 = numbers.every(num => num > 0);

// Solução 2:
const areAllPositive2 = numbers.every(function(num) {
  return num > 0;
});
```

**8. Dado um array de nomes, utilize o método `join` para criar uma string única com todos os nomes separados por vírgula.**

```javascript
// Solução 1:
const names = ['Alice', 'Bob', 'Charlie'];
const namesString1 = names.join(', ');

// Solução 2:
const namesString2 = names.join(', ');
```

**9. Crie um array de strings e utilize o método `concat` para adicionar mais uma string ao final.**

```javascript
// Solução 1:
const fruits1 = ['apple', 'banana', 'cherry'];
const newFruits1 = fruits1.concat('date');

// Solução 2:
const newFruits2 = fruits1.concat('date');
```

**10. Escreva uma função que recebe um array de números e retorna o maior e o menor número do array em um novo array.**

```javascript
// Solução 1:
function getMinMax1(array) {
  const min = Math.min(...array);
  const max = Math.max(...array);
  return [min, max];
}

// Solução 2:
const getMinMax2 = function(array) {
  const min = Math.min(...array);
  const max = Math.max(...array);
  return [min, max];
};
```

**11. Crie um array de números e utilize o método `indexOf` para encontrar a posição do número 15.**

```javascript
// Solução 1:
const numbers = [10, 5, 15, 20, 25];
const index1 = numbers.indexOf(15);

// Solução 2:
const index2 = numbers.indexOf(15);
```

**12. Dado um array de palavras, utilize o método `lastIndexOf` para encontrar a última posição da palavra "banana".**

```javascript
// Solução 1:
const words = ['apple', 'banana', 'cherry', 'banana', 'date'];
const lastIndex1 = words.lastIndexOf('banana');

// Solução 2:
const lastIndex2 = words.lastIndexOf('banana');
```

**13. Crie um array de objetos, onde cada objeto representa um aluno (com propriedades como nome, nota, etc.). Utilize o método `find` para encontrar o aluno com a maior nota.**

```javascript
// Solução 1:
const students = [
  { name: 'Alice', grade: 90 },
  { name: 'Bob', grade: 85 },
  { name: 'Charlie', grade: 95 }
];
const topStudent1 = students.find(student => student.grade === Math.max(...students.map(s => s.grade)));

// Solução 2:
const topStudent2 = students.find(function(student) {
  return student.grade === Math.max(...students.map(s => s.grade));
});
```

**14. Escreva uma função que recebe um array de números e retorna um novo array com os números em ordem crescente.**

```javascript
// Solução 1:
function sortNumbersAscending1(array) {
  return array.slice().sort((a, b) => a - b);
}

// Solução 2:
const sortNumbersAscending2 = function(array) {
  return array.slice().sort((a, b) => a - b);
};
```

**15. Dado um array de strings, utilize o método `includes` para verificar se a palavra "JavaScript" está presente.**

```javascript
// Solução 1:
const strings = ['HTML', 'CSS', 'JavaScript', 'Node.js'];
const hasJavaScript1 = strings.includes('JavaScript');

// Solução 2:
const hasJavaScript2 = strings.includes('JavaScript');
```

**16. Crie um array de números e utilize o método `toString` para transformar o array em uma string.**

```javascript
// Solução 1:
const numbers = [1, 2, 3, 4, 5];
const numbersString1 = numbers.toString();

// Solução 2:
const numbersString2 = numbers.toString();
```

**17. Dado um array de números, utilize o método `isArray` para verificar se é realmente um array.**

```javascript
// Solução 1:
const array1 = [1, 2, 3];
const isArray1 = Array.isArray(array1);

// Solução 2:
const array2 = [1, 2, 3];
const isArray2 = Array.isArray(array2);
```

**18. Crie um array de strings e utilize o método `slice` para pegar uma porção do array (por exemplo, os primeiros 3 elementos).**

```javascript
// Solução 1:
const strings1 = ['apple', 'banana', 'cherry', 'date', 'elderberry'];
const slicedStrings1 = strings1.slice(0, 3);

// Solução 2:
const slicedStrings2 = strings1.slice(0, 3);
```

**19. Escreva uma função que recebe um array de números e um número alvo, e retorna um novo array com os números maiores que o alvo.**

```javascript
// Solução 1:
function filterNumbersGreaterThanTarget1(array, target) {
  return array.filter(num => num > target);
}

// Solução 2:
const filterNumbersGreaterThanTarget2 = function(array, target) {
  return array.filter(num => num > target);
};
```

**20. Crie um array de strings e utilize o método `splice` para substituir uma string por outra em uma posição específica.**

```javascript
// Solução 1:
const fruits1 = ['apple', 'banana', 'cherry'];
fruits1.splice(1, 1, 'pear'); // Substitui 'banana' por 'pear'

// Solução 2:
const fruits2 = ['apple', 'banana', 'cherry'];
fruits2.splice(1, 1, 'pear');
```

**21. Dado um array de objetos, onde cada objeto representa um livro (com propriedades como título, autor, etc.), utilize o método `map` para criar um novo array com os títulos dos livros.**

```javascript
// Solução 1:
const books = [
  { title: 'The Great Gatsby', author: 'F. Scott Fitzgerald' },
  { title: 'To Kill a Mockingbird', author: 'Harper Lee' },
  { title: '1984', author: 'George Orwell' }
];
const bookTitles1 = books.map(book => book.title);

// Solução 2:
const bookTitles2 = books.map(function(book) {
  return book.title;
});
```

**22. Crie um array de números e utilize o método `filter` para retornar somente os números ímpares.**

```javascript
// Solução 1:
const numbers = [1, 2, 3, 4, 5];
const oddNumbers1 = numbers.filter(num => num % 2 !== 0);

// Solução 2:
const oddNumbers2 = numbers.filter(function(num
ChatGPT
) {
  return num % 2 !== 0;
});
```

**23. Escreva uma função que recebe um array de strings e retorna um novo array com as strings ordenadas por ordem alfabética.**

```javascript
// Solução 1:
function sortStringsAlphabetically1(array) {
  return array.slice().sort();
}

// Solução 2:
const sortStringsAlphabetically2 = function(array) {
  return array.slice().sort();
};
```

**24. Dado um array de números, utilize o método `reduce` para calcular o produto de todos os elementos.**

```javascript
// Solução 1:
const numbers = [1, 2, 3, 4, 5];
const product1 = numbers.reduce((accumulator, num) => accumulator * num, 1);

// Solução 2:
const product2 = numbers.reduce(function(accumulator, num) {
  return accumulator * num;
}, 1);
```

**25. Crie um array de objetos, onde cada objeto representa uma pessoa (com propriedades como nome, idade, etc.). Utilize o método `every` para verificar se todas as pessoas são maiores de idade.**

```javascript
// Solução 1:
const people = [
  { name: 'Alice', age: 25 },
  { name: 'Bob', age: 17 },
  { name: 'Charlie', age: 32 }
];
const areAllAdults1 = people.every(person => person.age >= 18);

// Solução 2:
const areAllAdults2 = people.every(function(person) {
  return person.age >= 18;
});
```

**26. Crie um array de strings e utilize o método `join` para criar uma única string com todas as palavras separadas por espaço.**

```javascript
// Solução 1:
const words1 = ['Hello', 'world', 'of', 'JavaScript'];
const sentence1 = words1.join(' ');

// Solução 2:
const sentence2 = words1.join(' ');
```

**27. Dado um array de números, utilize o método `concat` para adicionar mais um array de números ao final.**

```javascript
// Solução 1:
const numbers1 = [1, 2, 3];
const moreNumbers1 = [4, 5, 6];
const combinedNumbers1 = numbers1.concat(moreNumbers1);

// Solução 2:
const combinedNumbers2 = numbers1.concat(moreNumbers1);
```

**28. Escreva uma função que recebe um array de números e retorna um novo array com os números em ordem reversa.**

```javascript
// Solução 1:
function reverseNumbers1(array) {
  return array.slice().reverse();
}

// Solução 2:
const reverseNumbers2 = function(array) {
  return array.slice().reverse();
};
```

**29. Dado um array de objetos, onde cada objeto representa um animal (com propriedades como nome, espécie, etc.), utilize o método `filter` para retornar somente os animais que são aves.**

```javascript
// Solução 1:
const animals = [
  { name: 'Eagle', species: 'Bird' },
  { name: 'Lion', species: 'Mammal' },
  { name: 'Sparrow', species: 'Bird' }
];
const birds1 = animals.filter(animal => animal.species === 'Bird');

// Solução 2:
const birds2 = animals.filter(function(animal) {
  return animal.species === 'Bird';
});
```

**30. Crie um array de números e utilize o método `includes` para verificar se o número 7 está presente.**

```javascript
// Solução 1:
const numbers = [1, 3, 5, 7, 9];
const hasSeven1 = numbers.includes(7);

// Solução 2:
const hasSeven2 = numbers.includes(7);
```

**31. Crie um array de strings e utilize o método `toString` para transformar o array em uma única string, separando as strings por ponto-e-vírgula.**

```javascript
// Solução 1:
const strings1 = ['apple', 'banana', 'cherry'];
const joinedString1 = strings1.toString(';');

// Solução 2:
const joinedString2 = strings1.toString(';');
```

**32. Escreva uma função que recebe um array de números e retorna a média dos valores.**

```javascript
// Solução 1:
function calculateAverage1(array) {
  const sum = array.reduce((accumulator, num) => accumulator + num, 0);
  return sum / array.length;
}

// Solução 2:
const calculateAverage2 = function(array) {
  const sum = array.reduce(function(accumulator, num) {
    return accumulator + num;
  }, 0);
  return sum / array.length;
};
```

**33. Dado um array de objetos, onde cada objeto representa um jogo (com propriedades como título, gênero, plataforma, etc.), utilize o método `filter` para retornar somente os jogos de tiro.**

```javascript
// Solução 1:
const games = [
  { title: 'Call of Duty', genre: 'Shooter', platform: 'PS4' },
  { title: 'Super Mario', genre: 'Platformer', platform: 'Switch' },
  { title: 'Counter-Strike', genre: 'Shooter', platform: 'PC' }
];
const shooterGames1 = games.filter(game => game.genre === 'Shooter');

// Solução 2:
const shooterGames2 = games.filter(function(game) {
  return game.genre === 'Shooter';
});
```

**34. Crie um array de números e utilize o método `reduce` para encontrar o maior valor.**

```javascript
// Solução 1:
const numbers = [12, 56, 34, 78, 21];
const maxNumber1 = numbers.reduce((max, num) => (num > max ? num : max), numbers[0]);

// Solução 2:
const maxNumber2 = numbers.reduce(function(max, num) {
  return num > max ? num : max;
}, numbers[0]);
```

**35. Dado um array de strings, utilize o método `every` para verificar se todas as strings têm mais de 3 caracteres.**

```javascript
// Solução 1:
const strings = ['cat', 'dog', 'elephant', 'lion'];
const allHaveMoreThanThreeChars1 = strings.every(str => str.length > 3);

// Solução 2:
const allHaveMoreThanThreeChars2 = strings.every(function(str) {
  return str.length > 3;
});
```

**36. Escreva uma função que recebe um array de strings e um caractere, e retorna um novo array com as strings que contêm o caractere.**

```javascript
// Solução 1:
function filterStringsContainingChar1(array, char) {
  return array.filter(str => str.includes(char));
}

// Solução 2:
const filterStringsContainingChar2 = function(array, char) {
  return array.filter(str => str.includes(char));
};
``
ChatGPT
`

**37. Crie um array de objetos, onde cada objeto representa um filme (com propriedades como título, ano, diretor, etc.). Utilize o método `map` para criar um novo array com os diretores dos filmes.**

```javascript
// Solução 1:
const movies = [
  { title: 'Inception', year: 2010, director: 'Christopher Nolan' },
  { title: 'Avatar', year: 2009, director: 'James Cameron' },
  { title: 'The Matrix', year: 1999, director: 'The Wachowskis' }
];
const directors1 = movies.map(movie => movie.director);

// Solução 2:
const directors2 = movies.map(function(movie) {
  return movie.director;
});
```

**38. Dado um array de números, utilize o método `filter` para retornar somente os números que são divisíveis por 3.**

```javascript
// Solução 1:
const numbers = [9, 12, 15, 20, 25];
const divisibleByThree1 = numbers.filter(num => num % 3 === 0);

// Solução 2:
const divisibleByThree2 = numbers.filter(function(num) {
  return num % 3 === 0;
});
```

**39. Escreva uma função que recebe um array de strings e retorna um novo array com as strings em caixa alta.**

```javascript
// Solução 1:
function convertToUpperCase1(array) {
  return array.map(str => str.toUpperCase());
}

// Solução 2:
const convertToUpperCase2 = function(array) {
  return array.map(function(str) {
    return str.toUpperCase();
  });
};
```

**40. Crie um array de números e utilize o método `slice` para pegar uma porção do array (por exemplo, do terceiro ao quinto elemento).**

```javascript
// Solução 1:
const numbers1 = [10, 20, 30, 40, 50, 60, 70];
const portion1 = numbers1.slice(2, 5);

// Solução 2:
const portion2 = numbers1.slice(2, 5);
```

**41. Dado um array de objetos, onde cada objeto representa um país (com propriedades como nome, população, etc.), utilize o método `some` para verificar se existe algum país com população acima de 100 milhões.**

```javascript
// Solução 1:
const countries = [
  { name: 'USA', population: 331_002_651 },
  { name: 'China', population: 1_439_323_776 },
  { name: 'Brazil', population: 209_288_278 }
];
const hasCountryWithHighPopulation1 = countries.some(country => country.population > 100_000_000);

// Solução 2:
const hasCountryWithHighPopulation2 = countries.some(function(country) {
  return country.population > 100_000_000;
});
```

**42. Crie um array de strings e utilize o método `splice` para remover uma string em uma posição específica.**

```javascript
// Solução 1:
const fruits1 = ['apple', 'banana', 'cherry'];
fruits1.splice(1, 1); // Remove 'banana'

// Solução 2:
const fruits2 = ['apple', 'banana', 'cherry'];
fruits2.splice(1, 1);
```

**43. Escreva uma função que recebe um array de números e retorna um novo array com os números em ordem decrescente.**

```javascript
// Solução 1:
function sortNumbersDescending1(array) {
  return array.slice().sort((a, b) => b - a);
}

// Solução 2:
const sortNumbersDescending2 = function(array) {
  return array.slice().sort((a, b) => b - a);
};
```

**44. Dado um array de números, utilize o método `join` para criar uma única string com todos os números separados por vírgula.**

```javascript
// Solução 1:
const numbers1 = [10, 20, 30, 40, 50];
const joinedNumbers1 = numbers1.join(', ');

// Solução 2:
const joinedNumbers2 = numbers1.join(', ');
```

**45. Crie um array de objetos, onde cada objeto representa um funcionário (com propriedades como nome, cargo, salário, etc.). Utilize o método `every` para verificar se todos os funcionários ganham mais de R$ 5000,00.**

```javascript
// Solução 1:
const employees = [
  { name: 'Alice', position: 'Manager', salary: 6000 },
  { name: 'Bob', position: 'Developer', salary: 5500 },
  { name: 'Charlie', position: 'Designer', salary: 4800 }
];
const allEarnMoreThan50001 = employees.every(employee => employee.salary > 5000);

// Solução 2:
const allEarnMoreThan50002 = employees.every(function(employee) {
  return employee.salary > 5000;
});
```

**46. Dado um array de strings, utilize o método `indexOf` para verificar se a palavra "banana" está presente.**

```javascript
// Solução 1:
const strings1 = ['apple', 'banana', 'cherry'];
const hasBanana1 = strings1.indexOf('banana') !== -1;

// Solução 2:
const hasBanana2 = strings1.indexOf('banana') !== -1;
```

**47. Crie um array de números e utilize o método `concat` para adicionar mais um número ao final.**

```javascript
// Solução 1:
const numbers1 = [1, 2, 3];
const newNumbers1 = numbers1.concat(4);

// Solução 2:
const newNumbers2 = numbers1.concat(4);
```

**48. Escreva uma função que recebe um array de strings e um caractere, e retorna um novo array com as strings que contêm o caractere.**

```javascript
// Solução 1:
function filterStringsContainingChar1(array, char) {
  return array.filter(str => str.includes(char));
}

// Solução 2:
const filterStringsContainingChar2 = function(array, char) {
  return array.filter(str => str.includes(char));
};
```

**49. Dado um array de objetos, onde cada objeto representa um jogo (com propriedades como título, gênero, plataforma, etc.), utilize o método `filter` para retornar somente os jogos de tiro.**

```javascript
// Solução 1:
const games = [
  { title: 'Call of Duty', genre: 'Shooter', platform: 'PS4' },
  { title: 'Super Mario', genre: 'Platformer', platform: 'Switch' },
  { title: 'Counter-Strike', genre: 'Shooter', platform: 'PC' }
];
const shooterGames1 = games.filter(game => game.genre === 'Shooter');

// Solução 2:
const shooterGames2 = games.filter(function(game
ChatGPT
) {
  return game.genre === 'Shooter';
});
```

**50. Crie um array de strings e utilize o método `toString` para transformar o array em uma única string, separando as strings por ponto-e-vírgula.**

```javascript
// Solução 1:
const strings1 = ['apple', 'banana', 'cherry'];
const joinedString1 = strings1.toString(';');

// Solução 2:
const joinedString2 = strings1.toString(';');
```

Espero que essas soluções alternativas ajudem a aprofundar ainda mais sua compreensão dos conceitos e métodos em JavaScript! Se tiver mais dúvidas ou quiser mais exemplos, sinta-se à vontade para perguntar.

