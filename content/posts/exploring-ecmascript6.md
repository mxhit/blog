---
title: "Exploring ECMAScript6"
date: 2022-03-28T17:47:19+05:30
draft: false
---
In my almost three years of experience as a Java developer, I have hardly been exposed to working with front-end technologies. A little JSP here, a tad bit of CSS there, and the occasional `$("#div").modal()` while debugging to check whether my modals were showing up correctly or not. In conclusion, very elementary. However, I switched my job after two years and currently I am working with a legacy application that employs Core Java for the back-end and Angular.js for the front-end. This new project has given me a wonderful opportunity to learn JavaScript and I have truly begun to appreciate its beauty.

Learning JavaScript was not much of a hassle when compared to Java. I came across some wonderful resources that gave me a deep understanding of how the language works. One such resource was [freeCodeCamp’s JavaScript curriculum](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/). You will find some of my favourite features from ES6 listed below.

### Constant

Coming from Java, this feels like a familiar hug. Constants are immutable variables which cannot be reassigned new value(s). This means you can freely manipulate content of the constant variable but cannot redefine it with some new value.
```javascript
const arr = [1, 2, 3];
arr[1] += 5; // manipulating the value
console.log(arr); // prints [1, 7, 3]
arr = [2, 5, 7]; // throws Uncaught TypeError: invalid assignment to const ‘arr’
```

### Block-scoped Variables (a.k.a. `let` variables)

Another feature which will make a Java developer feel right at home. These variables, defined with the keyword let, have the scope of the block they are defined in.
```javascript
let i = 1;

{
    let i = 10;
    console.log(i); // prints 10
}

console.log(i); // prints 1
```

### Arrow Functions

One of the most prominent and well-accepted changes is the ability to create anonymous functions using the arrow notation. This change is single-handedly responsible for clearing the clutter that anonymous functions used to create.

```javascript
// Without Arrow function
var isEven = function(num) {
 return num % 2 === 0;
}

// With Arrow function
const isEven = (num) => num % 2 === 0;
```

Look at that! Clean and concise.

### Spread Operator

Contrary to the Rest Parameter, this operator allows us to spread the elements of an iterable collection, like an array or string.

```javascript
let str = “spread”;
let chars = [ …str ]; // [ “s”, “p”, “r”, “e”, “a”, “d” ];
```

### Template Literals

Template Literals, a. k. a. Template Strings, allows you to directly use a literal in an expression. The best example of a use-case is when you want to log something in the console.

```javascript
require(‘dotenv’).config();

const express = require(‘express’);
const app = express();
const port = process.env.PORT;

app.listen(port, () => console.log(`Server is listening on port ${port}`));
```

No more appending literals using the + operator.

### Property Shorthand

Like Arrow Functions, this new change allows us to define objects more easily in a simple and concise fashion.

```javascript
// Before
let x = 0, y = 0;
obj = { x: x, y: y };

// After
let x = 0, y = 0;
obj = { x, y };
```
---

There are considerably more new features in ES6 like Promises, Export, Classes, etc., which are of great significance while writing JavaScript code today. However, these topics require a lot more context and information, which does not fall into the scope of this blog — which is supposed to be a brief list of things that I liked the most.