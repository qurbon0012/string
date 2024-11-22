1. Создание строк
В JavaScript строки можно создавать несколькими способами:

Используя одинарные кавычки:



let str1 = 'Hello, World!';
Используя двойные кавычки:


let str2 = "JavaScript is awesome!";
Используя обратные кавычки (template literals) — удобны для вставки переменных и многострочных строк:


let name = 'Alice';
let greeting = `Hello, ${name}!`;  // Интерполяция переменных
Также обратные кавычки позволяют создавать многострочные строки:


let multilineString = `This is
a multi-line
string.`;
2. Основные операции с строками
Конкатенация (объединение строк): Для объединения строк используется оператор + или метод .concat():


let str1 = 'Hello';
let str2 = 'World';
let result = str1 + ' ' + str2;  // "Hello World"
Доступ к символам строки: Для получения символа по индексу используется синтаксис [index]:


let str = 'Hello';
let char = str[1];  // 'e'
Для получения позиции символа используется метод .indexOf():


let position = str.indexOf('e');  // 1
Длина строки: Метод .length возвращает количество символов в строке:


let str = 'Hello';
let length = str.length;  // 5
3. Методы работы со строками
toUpperCase() — преобразует строку в верхний регистр:


let str = 'hello';
let upperStr = str.toUpperCase();  // "HELLO"
toLowerCase() — преобразует строку в нижний регистр:


let str = 'HELLO';
let lowerStr = str.toLowerCase();  // "hello"
trim() — удаляет пробелы с начала и конца строки:


let str = '  hello  ';
let trimmedStr = str.trim();  // "hello"
slice() — извлекает подстроку из строки:


let str = 'Hello, World!';
let slicedStr = str.slice(0, 5);  // "Hello"
replace() — заменяет часть строки:


let str = 'Hello, World!';
let newStr = str.replace('World', 'JavaScript');  // "Hello, JavaScript!"
split() — разбивает строку на массив подстрок:


let str = 'apple,banana,cherry';
let fruits = str.split(',');  // ["apple", "banana", "cherry"]
4. Шаблонные строки (Template Literals)
Шаблонные строки в JavaScript — это строки, заключенные в обратные кавычки (`). Они позволяют вставлять выражения в строку с помощью ${} и удобны для работы с многострочными строками.

Пример:
let name = 'Alice';
let age = 25;
let message = `Hello, my name is ${name} and I am ${age} years old.`;
console.log(message);  // "Hello, my name is Alice and I am 25 years old."
Шаблонные строки позволяют вставлять не только переменные, но и выражения:


let a = 5;
let b = 10;
let sumMessage = `The sum of ${a} and ${b} is ${a + b}.`;
console.log(sumMessage);  // "The sum of 5 and 10 is 15."
5. Работа с Unicode и символами
JavaScript строки поддерживают Unicode, что позволяет работать с международными символами и эмодзи:


let str = 'Привет, мир! 🌍';
console.log(str.length);  // 15 (включая эмодзи как один символ)
Для работы с Unicode символами можно использовать методы, такие как charCodeAt():


let str = 'A';
let code = str.charCodeAt(0);  // 65 (код символа 'A')
6. Шаблонные строки vs обычные строки
Основное отличие между обычными строками (в кавычках) и шаблонными строками:

Шаблонные строки позволяют работать с переменными и выражениями через ${}.
Шаблонные строки также могут быть многострочными, в отличие от обычных строк, которые не могут содержать переносы строк без использования специальных символов (например, \n).
Пример:


let greeting = "Hello";
let name = "Bob";
let message = `${greeting}, ${name}!`;
console.log(message);  // "Hello, Bob!"
Заключение
Строки в JavaScript — это мощный инструмент для работы с текстовой информацией. Они поддерживают множество методов и функций для манипуляции текстом, что делает их незаменимыми при разработке приложений. С помощью строк можно не только хранить и отображать текст, но и выполнять сложные операции, такие как форматирование, поиск и замена текста.




# string
