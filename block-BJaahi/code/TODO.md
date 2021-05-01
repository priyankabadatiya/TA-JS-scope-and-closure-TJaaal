For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
var username = undefined;
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMesage = undefined;

// Execution Phase

console.log(username, numbers )

```

3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
let username;
let number;

let sayHello = function (name) {
return `Hello ${name}`;
};

let message;
var nextMessage = undefined;

// Execution Phase

console.log(username, numbers);

Uncaught ReferenceError: numbers is not defined.

```

4.

```js
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
//Declaration Phase

let username;
let number;
let message;
let sayHello;
var nextMessage = undefined;

```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
var name = undefined;
let age;
console.log(undefined);
// Uncaught ReferenceError: age is not defined.
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
// Declaration

function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = "Lydia";
  let age = 21;
}

sayHi();

```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
// Declaration

function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = "Lydia";
  let age = 21;
}

// Execution
//  Uncaught ReferenceError: Cannot access 'age' before initialization
```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
// Declaration

let sayHi;

// Execution

// Uncaught ReferenceError: sayHi is not defined
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
// Declaration

let num1;
var sum = undefined;
let num2;

// Execution
num1 = 21;
console.log(sum);
//  Uncaught ReferenceError: num2 is not defined
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
// Declaration

var num1 = undefined;
let sum2;
let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let add;
let num;
let sum;

// Execution

num1 = 21;

//  Uncaught ReferenceError: addAgain is not defined
```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
// Declaration

function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum;s
let add;

// Execution

// Uncaught ReferenceError: addAgain is not defined
```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
// Declaration

function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum;

function add(a, b) {
  return a + b;
}
```
