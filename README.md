**Interview-questions**

# HTML

### 1. What is HTML

HTML stands for Hypertext Markup Language. It's a markup language used to create web pages. HTML defines the structure and appearance of web pages, and how to display content.

### What is a Tag in HTML? Can you define HTML attributes?

### What is the key difference between HTML Elements and Tags? Also, Can you separate sections of texts in HTML?

### If you want to display some HTML data in a table in tabular format, which HTML tags will you use?

### What are Attributes in HTML?

### What is an Anchor tag in HTML?

### What are Lists in HTML?

### Define HTML Layout.

### What are Forms in HTML?

### What is the Use of Comments in HTML?

### What is HTML5?

### What is Semantic HTML?

### What is an Image Map?

### Why is the Embed Tag Used in HTML?

### What is a ‘Marquee’ Tag in HTML?


# JavaScript

## JavaScript fundamentals

=> JS-01

### 1. What is Javascript?

Javascript is a programming language that is used for converting static web pages to interactive and dynamic. 

### 2. What are JavaScript Data Types?

There are two category of data type: **1.** Primitive data type, **2.** Non-primitive/Reference data type

**Primitive data type:** Primitive data types are the most basic data types. Primitive data types are immutable and represents a single value. 
1. String
2. Number
3. Boolean
4. Null
5. Undefined
6. BigInt
7. Symbol

**Non-primitive/Reference data type:** Non-primitive data types are complex and mutable data types. They store collection of values in a variable.
1. Object
2. Array

### 3. What is the difference between primitive and non-primitive data types?

| Primitive    | Non-primitive |
| -------- | ------- |
| Primitive data types are string, number, boolean, null, undefined, symbol  | Non-primitive data types are object, array, function |
| Primitive data types are immutable means their value can not be changed. | Non-primitive data types are mutable means their value can be changed.    |
| Primitive data type represents only a single value    | Not-primitive data type represents multiple with collection of elements or a key value pair    |
| Primitive data types are simple data types  | Non-primitive data types are complex (means we can do multiple operation) data types

### 4. What are arrays, function and objects?

**Array:** An array is a special type of object used to store multiple values in a single variable. Unlike many other programming languages, JavaScript arrays are dynamic, meaning they can grow or shrink in size as needed. Arrays in JavaScript are zero-indexed, meaning the first element is at index 0, the second element is at index 1, and so on.

**Creating Arrays:**
We can create arrays in JavaScript using array literal syntax ([]) or the Array constructor.

```javascript

// Array literal syntax
let fruits = ['apple', 'banana', 'orange'];

// Array constructor
let cars = new Array('Toyota', 'Honda', 'Ford');
```
**Accessing Elements:**
We can access elements in an array using square brackets ([]) notation with the index of the element.

```javascript
console.log(fruits[0]); // Output: 'apple'
console.log(cars[1]);   // Output: 'Honda'
```
**Modifying Elements:**
We can modify elements in an array by assigning a new value to a specific index.

```javascript

fruits[2] = 'grape';
console.log(fruits); // Output: ['apple', 'banana', 'grape']
```
**Array Methods:**
JavaScript provides a variety of methods to manipulate arrays, such as **push(), pop(), shift(), unshift(), splice(), slice(), concat(), indexOf(), forEach(), map(), filter(), reduce()**, and many more.

```javascript
fruits.push('kiwi'); // Add 'kiwi' to the end of the array
console.log(fruits); // Output: ['apple', 'banana', 'grape', 'kiwi']

fruits.pop(); // Remove the last element from the array
console.log(fruits); // Output: ['apple', 'banana', 'grape']
```
**Array Length:**
We can determine the length of an array using the length property.

```javascript
console.log(fruits.length); // Output: 3
```
**Iterating Over Arrays:**
We can iterate over arrays using loops such as for loop or array methods like forEach(), map(), filter(), etc.

```javascript
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}

fruits.forEach(function(fruit) {
  console.log(fruit);
});
```

**Function:** A function is a block of code that performs a specific task and return a value. Functions are one of the fundamental building blocks of JavaScript programming, allowing us to encapsulate logic, organize code, and promote reusability.

**Creating Functions:**
You can define functions in JavaScript using either function declaration syntax or function expression syntax.

**Function Declaration:**

```javascript
function greet(name) {
  console.log('Hello, ' + name + '!');
}
```
**Function Expression (Anonymous Function):**

```javascript
let greet = function(name) {
  console.log('Hello, ' + name + '!');
};
```
**Function Parameters:**
Functions can accept input parameters (arguments) that are specified within the parentheses following the function name. These parameters represent values that can be passed to the function when it is called.

```javascript
function add(a, b) {
  return a + b;
}
```
**Calling Functions:**
To execute a function and perform its defined task, you need to call (invoke) it by using its name followed by parentheses. If the function expects parameters, you provide values for those parameters inside the parentheses.

```javascript
greet('Alice'); // Output: Hello, Alice!
let result = add(3, 5); // result is assigned the value 8
```
**Returning Values:**
Functions can optionally return a value using the return statement. This allows the function to calculate a result or perform some operation and then pass that result back to the calling code.

```javascript
function multiply(x, y) {
  return x * y;
}
let product = multiply(2, 4); // product is assigned the value 8
```
**Function Scope:**
JavaScript functions have their own scope, meaning that variables declared inside a function are local to that function and are not accessible from outside the function (unless explicitly returned).

**Function Hoisting:**
In JavaScript, function declarations are hoisted to the top of their containing scope, meaning you can call a function before it is declared in the code.

**First-Class Citizens:**
In JavaScript, functions are treated as first-class citizens, meaning they can be assigned to variables, passed as arguments to other functions, and returned from other functions, just like any other data type.

**Object:** An object is a collection of key-value pairs where each key is a unique identifier (also known as a property name) and each value is associated with that key. Objects are one of the core data types in JavaScript and are used to represent complex data structures and entities.

**Creating Objects:**
You can create objects in JavaScript using object literal syntax {} or the Object constructor.

**Object Literal Syntax:**

```javascript
let person = {
  name: 'John',
  age: 30,
  city: 'New York'
};
```
**Object Constructor:**

```javascript
let person = new Object();
person.name = 'John';
person.age = 30;
person.city = 'New York';
```
**Accessing Object Properties:**
You can access properties of an object using dot notation (.) or bracket notation ([]).

```javascript
console.log(person.name); // Output: 'John'
console.log(person['age']); // Output: 30
```
**Adding and Modifying Properties:**
You can add new properties or modify existing properties of an object after its creation.

```javascript
person.job = 'Engineer'; // Adding a new property
person.age = 35; // Modifying an existing property
```
**Nested Objects:**
Objects can contain other objects as property values, allowing you to create nested or hierarchical data structures.

```javascript
let car = {
  make: 'Toyota',
  model: 'Camry',
  year: 2020,
  owner: {
    name: 'Alice',
    age: 25
  }
};
```
**Object Methods:**
In JavaScript, functions can also be properties of objects. When a function is a property of an object, it is called a method.

```javascript
let person = {
  name: 'John',
  greet: function() {
    console.log('Hello, ' + this.name + '!');
  }
};
person.greet(); // Output: 'Hello, John!'
```

### 5. What is scope in javascript?

**Scope:** Scope refers to the visibility and accessibility of variables within a particular part of the code during runtime. It determines where variables and functions are accessible and where they are not.

**Types of Scope in JavaScript:**
JavaScript has two main types of scope:

**Global Scope:**
Variables declared outside of any function or block have global scope. Global variables are accessible from anywhere in the code, including inside functions and blocks. They are accessible throughout the entire script, but they can be shadowed by local variables.

```javascript
let globalVar = 'I am global';

function foo() {
  console.log(globalVar); // Accessible
}
```
**Local Scope:**
Variables declared inside a function or block have local scope. Local variables are only accessible within the function or block in which they are declared. They are not accessible outside of the function or block.

```javascript
function bar() {
  let localVar = 'I am local';
  console.log(localVar); // Accessible
}

console.log(localVar); // Error: localVar is not defined
```

**Block Scope:**
Prior to ES6 (ECMAScript 2015), JavaScript only had function scope. With the introduction of let and const keywords in ES6, block scope was introduced. Variables declared with let and const have block scope, meaning they are only accessible within the block in which they are declared.

```javascript
if (true) {
  let blockVar = 'I am block scoped';
  console.log(blockVar); // Accessible
}

console.log(blockVar); // Error: blockVar is not defined
```
### 6. Difference between var and let keyword in javascript.

| Feature	| var	| let	| const |
| ------- | ------- | -------- | ------- |
| Scope |	Function scope  | Block scope |	Block scope |
|Hoisting |	Hoisted to the top of the function	|Hoisted to the top of the block	| Hoisted to the top of the block. |
|Re-declaration	| Allowed |	Not allowed |	Not allowed |
|Re-assignment |	Allowed |	Allowed |	Not allowed (unless the value is mutable)|
|Initialization |	Optional | Optional | Required
|Example |	``` var x = 10; if (true) { var y = 20; } console.log(x); console.log(y);``` |	```let x = 10; if (true) { let y = 20; }	console.log(x); console.log(y);```	|```const x = 10; if (true) { const y = 20; } console.log(x); console.log(y);```|

**Scope:**

var: Scoped to the nearest function block.
let: Scoped to the nearest enclosing block (commonly a statement, like a loop or an if block).
const: Also scoped to the nearest enclosing block, just like let.

**Hoisting:**

var: Hoisted to the top of the function. Variables declared with var are hoisted and initialized with undefined.
let: Hoisted to the top of the block but not initialized. You'll get a ReferenceError if you try to access the variable before the declaration.
const: Hoisted to the top of the block but not initialized. Same behavior as let.

**Re-declaration:**

var: Allows re-declaration within the same scope.
let: Does not allow re-declaration within the same scope.
const: Does not allow re-declaration within the same scope.

**Re-assignment:**

var: Allows re-assignment of values.
let: Allows re-assignment of values.
const: Does not allow re-assignment of values, but the value itself may be mutable (e.g., objects and arrays).

**Initialization:**

var: Initialization is optional.
let: Initialization is optional.
const: Requires initialization at the time of declaration.

### 7. What is loop? What are loops in javascript?

A loop is a basic programming concept that allows us to execute a block of code repeatedly based on a condition. It's enable automation of repetitive tasks.

JavaScript supports several types of loops:

**for Loop:**
The for loop is used when you know the number of iterations in advance. It consists of three parts: initialization, condition, and iteration.

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```
**while Loop:**
The while loop is used when the number of iterations is not known in advance, and the loop continues as long as the specified condition is true.

```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```
**do...while Loop:**
The do...while loop is similar to the while loop, but it always executes the block of code at least once, even if the condition evaluates to false initially.

```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```
**for...in Loop:**
The for...in loop iterates over the enumerable properties of an object, including its prototype chain. It's commonly used to iterate over object keys.

```javascript
const person = { name: 'John', age: 30 };
for (const key in person) {
  console.log(key + ': ' + person[key]);
}
```
**for...of Loop:**
The for...of loop is used to iterate over iterable objects such as arrays, strings, and other iterable objects introduced in ES6.

```javascript
const colors = ['red', 'green', 'blue'];
for (const color of colors) {
  console.log(color);
}
```

### 8. Difference between “ == “ and “ === “ operators.

Both == (equality operator) and === (strict equality operator) are used for comparison, but they have different behaviors:

**== (Equality Operator):**

The == operator checks for equality after performing type coercion. If the operands have different types, JavaScript will attempt to convert them to the same type before making the comparison.

Example: 0 == false evaluates to true because false is converted to 0 during comparison.

**=== (Strict Equality Operator):**

The === operator checks for strict equality without performing type coercion. It only returns true if the operands are of the same type and have the same value.

Example: 0 === false evaluates to false because 0 and false are of different types.

**Here's a comparison table to illustrate the differences:**

|	Example |	Result |
| ------- | ------- |
|	0 == false | true |
| 0 === false | false |
|	"1" == 1|	true|	
|	"1" === 1|	false|
|null == undefined|	true|
|	null === undefined|	false|

=> Js-02

### 1. What are the types of functions? What are named and anonymous functions?
### 2. What is function expression?
### 3. What are arrow function?
### 4. What are callback functions?
### 5. When to use callback function in real application?
### 6. What is the use of event handling?
### 7. What is higher order functions?

=> Js-03

### 1. What are asynchronous operations?
### 2. What are promise?
### 3. How to implement promise
### 4. When to use promises in real application?
### 5. What are classes and objects?
### 6. What is the purpose of this keyword?
### 7. What is hoisting?


### 2. What is the use of isNaN function?
### 5. Explain Implicit Type Coercion in javascript.
### 6. Is javascript a statically typed or a dynamically typed language?
### 7. What is NaN property in JavaScript?
### 8. Explain passed by value and passed by reference.
### 9. What do you mean by strict mode in javascript and characteristics of javascript strict-mode?
### 10. Explain Higher Order Functions in javascript?
### 11. What is an Immediately Invoked Function in JavaScript?
### 12. Explain “this” keyword.
### 13. What do you mean by Self Invoking Functions?
### 14. Explain call(), apply() and, bind() methods.
### 15. What is currying in JavaScript?
### 16. What are some advantages of using External JavaScript?
### 17. Explain Scope and Scope Chain in javascript.
### 18. Explain Closures in JavaScript.
### 19. Mention some advantages of javascript.
### 20. What are object prototypes?
### 21. What are callbacks?
### 22. What are the types of errors in javascript?
### 23. What is memoization?
### 24. What is recursion in a programming language?
### 25. What is the use of a constructor function in javascript?
### 26. What is DOM?
### 27. Which method is used to retrieve a character from a certain index?
### 28. What do you mean by BOM?
### 29. What is the distinction between client-side and server-side JavaScript?
### 30. What are arrow functions?
### 31. What do mean by prototype design pattern?
### 32. Differences between declaring variables using var, let and const.
### 33. What is the rest parameter and spread operator?
### 34. In JavaScript, how many different methods can you make an object?
### 35. What is the use of promises in javascript?
### 36. What are classes in javascript?
### 37. What are generator functions?
### 38. Explain WeakSet in javascript.
### 39. Why do we use callbacks?
### 40. Explain WeakMap in javascript.
### 41. What is Object Destructuring?
### 42. Difference between prototypal and classical inheritance
### 43. What is a Temporal Dead Zone?
### 44. What do you mean by JavaScript Design Patterns?
### 45. Is JavaScript a pass-by-reference or pass-by-value language?
### 46. Difference between Async/Await and Generators usage to achieve the same functionality.
### 47. What are the primitive data types in JavaScript?
### 48. What is the role of deferred scripts in JavaScript?
### 49. What has to be done in order to put Lexical Scoping into practice?







## JavaScript behind the process.

### 1. How JavaScript Works?
### 2. What is Hoisting?
### 3. What is Temporal Dead Zone?
### 4. What is Event Loop?
### 5. What is scope and what scopes are available in JavaScript?
### 6. 


<!-- prettier-ignore-end -->
