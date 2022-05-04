## SimpleJavaScript
[![Simple JavaScript Banner](https://s3.amazonaws.com/freecodecamp/wide-social-banner.png)](https://github.com/signuldotdev/SimpleJavaScript/blob/main/README.md)

## SimpleJavaScript to brush up on your JavaScript skills

**JavaScript** (**JS**) is a lightweight, interpreted, or [just-in-time](https://en.wikipedia.org/wiki/Just-in-time_compilation) compiled programming language with [first-class functions](https://developer.mozilla.org/en-US/docs/Glossary/First-class_Function). 

JavaScript is a [prototype-based](https://developer.mozilla.org/en-US/docs/Glossary/Prototype-based_programming), multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional 
programming) styles.

## Table of Contents
## Getting Started ⇒ JavaScript Fundamentals


- [Table of Contents](#table-of-contents)
  - [Getting Started ⇒ JavaScript Fundamentals](#getting-started--javascript-fundamentals)
  - [JavaScript Fundamentals => Part 1](#javascript-fundamentals--part-1)
- [Hello World](#hello-world)
- [A Brief Introduction Of JavaScript](#a-brief-introduction-of-javascript)
- [Linking A JavaScript File](#linking-a-javascript-file)
- [Values & Variables](#values--variables)
- [Data Types](#data-types)
  - [The 7 Primitive Data Types](#the-7-primitive-data-types)
- [Let, Const & Var](#let-const--var)
- [Basic Operators](#basic-operators)
- [Operator Precedence](#operator-precedence)
- [String & Template literals](#string--template-literals)
- [Taking Decisions: If / Else statements](#taking-decisions-if--else-statements)
- [Type Conversion & Coercion](#type-conversion--coercion)
- [Truthy & Falsy Values](#truthy--falsy-values)
- [Equality Operator == vs ===](#equality-operator--vs-)
- [Boolean Logic : The AND, OR & NOT Operators](#boolean-logic--the-and-or--not-operators)
- [Logical Operators](#logical-operators)

- [JavScript Fundamentals => Part - 2](javascript-fundamentals-part-2)
   - [Activating Strict Mode](#activating-strict-mode)
   - [Functions](#functions)

----

## JavaScript Fundamentals => Part 1

---- 

## Hello World

In your browser, Open developer console and go to console bracket and run:

```jsx
alert('Hello World!!!');
// Hello World!!!

console.log('Hello World!!!');
// Hello World!!!

let javascript = 'awesome'
// undefined
if (javascript === 'awesome') alert('JavaScript is Awesome!!!')

JavaScript is Awesome!!!
```

```jsx
23 + 27 + 21
71

28 * 76
2128

2 % 10
2
```

## A Brief Introduction Of JavaScript

What is JavaScript? 

- **`JavaScript is a high-level, object-oriented, multi-paradigm, programming language.`**
- Programming Language
    - Instruct Computer to do things
- Object-Oriented
    - Based on objects, for storing most kinds of data
- High-Level
    - We don't have to worry about complex stuff like memory management
- Multi-Paradigm
    - We can use different styles of programming

 

The Role of JavaScript in web development ?

- HTML

```jsx
NOUNS, 
		<p></p>
means "paragraph"
```

- CSS

```jsx
ADJECTIVES,
		p { color: red}
means "the paragraph text is red"
```

- JS

```jsx
VERBS,
		p.hide();
means "hide the paragraph"
```

There is nothing you can't do with JavaScript (WELL, ALMOST...)

- Front-End
    - React
    - Angular
    - Vue
- Back-End
    - Node JS
- Native Mobile Application
    - React Native
    - Ionic
- Native Desktop Application
    - Electron


## Linking A JavaScript File

- Add JavaScript to `index.html` file,

```html
<body>
    <h1>JavaScript Fundamentals – Part 1</h1>

    <script src="script.js"></script>
</body>
```

- Run code on `script.js` file,

```jsx
let js = 'amazing';   
if (js === 'amazing') alert('JavaScript is Awesome');

console.log(49 + 23 - 23 + 12);
```

```jsx
OUTPUT:

JavaScript is Awesome

CONSOLE:
61
```

## Values & Variables

<aside>
💡 `Variables` are containers for storing data (`values`).

</aside>

```jsx
let myCountry = 'India';
let myContinent = 'Asia';
let myPopulation = '1.36 Cr';

console.log(myCountry, myContinent, myPopulation);

// India Asia 1.36 Cr
```

## Data Types

In JS, every `value` is an `object` or `primitive` `Data` `Types`

- Object

```jsx
let me = {
	name: 'Jonas'
};
```

- Primitive

```jsx
let firstName = 'Jonas';
let age = 30;
```

### The 7 Primitive Data Types

1. `Number` : Floating point numbers 👉🏻 Used for decimals and integers 

```jsx
let age = 23;
```

1. `String` : Sequence of Characters 👉🏻  Used for text 

```jsx
let firstName = 'Jonas';
```

1. `Boolean` : Logical type that can only be true or false 👉🏻 Used for taking decisions 

```jsx
let fullAge = true;
```

1. `Undefined` : Value taken by a variable that is not yet defined('empty value')

```jsx
let children;
```

1. `Null` : Also means 'empty value'
2. `Symbol` (ES2015) : Value that is unique and cannot be changed [Not useful for now]
3. `BigInt` : (ES2020) : Larger integers than the Number type can hold

----
<aside>
💡 Commenting Code

</aside>

```jsx
// This is Single line comment
/* This is multi-line comment */
```
----

## Let, Const & Var

Let, Const & Var are the three different ways to declaring variables.

- `let` :

The `let` keyword was introduced in
[ES6 (2015)](https://www.w3schools.com/js/js_es6.asp).

Variables defined with `let` cannot be Redeclared.

Variables defined with `let` must be Declared before use.

Variables defined with `let` have Block Scope.

- `var` :

Variables are containers for storing data (values).

In this example, `x`, `y`, and `z`, are variables, declared with the `var` keyword:

```jsx
var x = 5;
var y = 6;
var z = x + y;

// 11
```

- `const` :

The `const` keyword was introduced in
[ES6 (2015)](https://www.w3schools.com/js/js_es6.asp).

Variables defined with `const` cannot be Redeclared.

Variables defined with `const` cannot be Reassigned.

Variables defined with `const` have Block Scope.

```jsx
const PI = 3.141592653589793;
PI = 3.14;      // This will give an error
PI = PI + 10;   // This will also give an error

// TypeError: invalid assignment to const 'PI'
```

## Basic Operators

```jsx
const now = 2021;
const ageVinit = now - 1996;
const ageSanket = now - 2000;
console.log(ageVinit, ageSanket);

// 25 21

console.log(ageVinit * 2, ageSanket + 2 * 2);

// 25, 50

const firstName = 'Sanket';
const lastName = 'Sangha';
console.log(firstName + ' ' + lastName);

// Sanket Sangha
```

## Operator Precedence

[Operator precedence](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence)` determines how operators are parsed concerning each other. Operators with higher precedence become the operands of operators with lower precedence.`


## String & Template literals

`**String` 👇🏻** 

<aside>
💡 Old Trick

</aside>

```jsx
const firstName = 'Sanket';
const job = 'teacher';
const birthYear = 2000;
const year = 2021;

const sanket = "I'm " + firstName + ', a ' + (year - birthYear) 
+ ' years old ' + job + '!';
console.log(sanket);

// I'm Sanket, a 21 years old teacher!
```

`**Template literals 👇🏻**`

*Template Literals use back-ticks (``) rather than the quotes ("") to define a string.*

<aside>
💡 New Trick

</aside>

```jsx
const firstName = 'Sanket';
const job = 'teacher';
const birthYear = 2000;
const year = 2021;

const newSanket = `I'm ${firstName}, a ${year - birthYear} 
year old ${job}!`;
console.log(newSanket);

// I'm Sanket, a 21 year old teacher!
```

## Taking Decisions: If / Else statements

`Example 1:`

```jsx
const age = 19; or const age = 15;

if (age >= 18) {
    console.log('Sanket can start driving license 🚗');
//  Sanket can start driving license 🚗
} else {
    const yearsLeft = 18 - age;
    console.log(`Sanket is too young. Wait another ${yearsLeft} years :)`);
}
// Sanket is too young. Wait another 3 years :)
```

`Example 2:`

```jsx
const year = 2021;

let birthYear;
if (birthYear <= 2000) {
    century = 20;
} else {
    century = 21;
}

console.log(century);

// 21
```

## Type Conversion & Coercion

`**Type Conversion` 👇🏻**

JavaScript variables can be converted to a new variable and another data type:

- By the use of a JavaScript function
- **Automatically** by JavaScript itself

```jsx
// Type conversion
const inputYear = 2000;
console.log(Number(inputYear), inputYear);
console.log(Number(inputYear) + 18);

console.log(Number('Sanket'));
console.log(typeof NaN);

console.log(String(23), 23);

// OUTPUT:
2000 2000 
2018
NaN 
number 
23 23
```

`**Type Coercion 👇🏻**`

Type Coercion refers **to the process of automatic or implicit conversion of values from one data type to another**.

```jsx
// Type Coercion
console.log('I am ' + 23 + ' year old');
console.log('23' - '10' - 3);
console.log('23' * '2');
console.log('23' > '18');

// OUTPUT:
I am 23 year old 
10 
46 
true
```


## Truthy & Falsy Values

Truthy -> Value that resolve to true in boolean context

Falsy -> Value that resolve to false in boolean context

**List of falsy values in JavaScript:**[From MDN](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

1. `false`
2. `null`
3. `undefined`
4. `0`
5. `NaN`
6. `''`, `""`, ````(Empty template string)
7. `document.all`
8. `0n`: BigInt
9. `0`


## Equality Operator == vs ===

The `equality operator == does type coercion,` meaning that the interpreter implicitly tries to convert the values before comparing.

The `identity operator === does not do type coercion,` and thus does not convert the values when comparing, and is therefore faster as it skips one step.

## Boolean Logic : The AND, OR & NOT Operators

A JavaScript Boolean represents one of two values: `true` or `false`.

`**Boolean Values**`

Very often, in programming, you will need a data type that can only have one 
of two values, like

- YES / NO
- ON / OFF
- TRUE / FALSE

For this, JavaScript has a **Boolean** data type. It can only 
take the values **true** or **false**.


## Logical Operators

[Logical operators](https://javascript.info/logical-operators) are used to determine the logic between variables or values.


## The Switch Statement

> The switch statement is used to perform different actions based on different conditions.
> 

> **`Syntax:`**
> 

```jsx
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

### Example

The `getDay()` method returns the weekday as a number between 
 0 and 6.

(Sunday=0, Monday=1, Tuesday=2 ..)

This example uses the weekday number to calculate the weekday name:

```jsx
switch (new Date().getDay()) {
  case 0:
    day = "Sunday";
    break;
  case 1:
    day = "Monday";
    break;
  case 2:
     day = "Tuesday";
    break;
  case 3:
    day = "Wednesday";
    break;
  case 4:
    day = "Thursday";
    break;
  case 5:
    day = "Friday";
    break;
  case 6:
    day = "Saturday";
}

// Saturday
```


## Statements & Expressions

- `**Statement`👇🏻**

> JavaScript statement are composed of:
> 

> Values, Operators, Expressions, Keywords, and Comments.
> 

```jsx
// This statement tells the browser to write "Hello Dolly." inside an HTML element with id="demo":

document.getElementById("demo").innerHTML = "Hello Dolly.";
```

- `**Expression 👇🏻**`

> An expression is a snippet of code that evaluates to a value.
> 

```jsx
// The below code snippets are all expressions. They all evaluate to a value.

0 // 0

1 + 1 // 2

'Hello' + ' ' + 'World' // 'Hello World'

{ answer: 42 } // { answer: 42 }

Object.assign({}, { answer: 42 }) // { answer: 42 }

answer !== 42 ? 42 : answer // 42

answer = 42 // 42
```


## The Conditional (Ternary) Operator

> The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark (?), then an expression to execute if the condition is `truthy` followed by a colon (:), and finally the expression to execute if the condition is `falsy`. This operator is frequently used as a shortcut for the if statement.
> 

```jsx
function getFee(isMember) {
  return (isMember ? '$2.00' : '$10.00');
}

console.log(getFee(true));
// expected output: "$2.00"

console.log(getFee(false));
// expected output: "$10.00"

console.log(getFee(null));
// expected output: "$10.00"
```

## JavaScript Release ES5, ES6+ & ESNext

> A Brief History of JavaScript
> 
- 1995 👉🏻 Brendan Eich very first version of javascript in just 10 days.
- 1996 👉🏻 JavaScript has almost nothing to do with Java.
- 1997 👉🏻 Official Standard for JavaScript
- 2009👉🏻 ES5 (ECMAScript 5) is released with lots of great new features.
- 2015👉🏻 ES6/ES2015 was released the biggest update to the language ever!
- 2016 - | 👉🏻 Release of ES2016/ES2017/ES2018/ES2019/ES2020/ES2021/ .../ ES2089 😂

> Backwards Compatibility: Don't Break the Web!
> 
- Backwards Compatibility
- Old features are never removed;
- Not really new versions, just incremental updates(releases)
- Websites keep working forever!

> How to use Modern JavaScript Today
> 
- During development 👉🏻 Simply use the latest Google Chrome!
- During production 👉🏻 Use Babel to transpile and polyfill your code (converting back to ES5 to ensure browser compatibility for all users).

---- 

# JavaScript Fundamentals- Part 2

## Activating Strict Mode

> `"use strict";` Defines that
JavaScript code should be executed in
"strict mode".
> 
- Always use strict mode on top of code.

```jsx
'use strict';
```

## Functions

```jsx
function Apple() {
	console.log('iphone is Apple Inc. Product');
}

Apple();
```