1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

var per = function percentage(marks, total) {
  return (marks * 100) / total;
}
var per = percentage(marks, total)=> {
  return (marks * 100) / total;
}


```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
var percent=function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
```js
const getRectArea = function(width, height) {
  return width * height;
};

console.log(getRectArea(3, 4));

4. Why is a function call an expression in JavaScript?
```js
A function call expression is used to execute a specified function with the provided arguments.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid
five = add; //valid
five = five(10, 11); // valid
five = function () {
  return 'Hello';
}; //valid
```

6. What is the difference between function definition and function call? Explain with an example.
``js
Using a function to do a particular task any point in program is called as function call. So the difference between the function and function call is, A function is procedure to achieve a particular result while function call is using this function to achive that task.

7. What is the similarities between function definition and function call?
```js

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid
```

9. What is higher order function explain with an example.
A Higher-Order function is a function that receives a function as an argument or returns the function as output. 

10. Explain what is callback function. Why you can pass a function inside a function?
```js
A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.
partial accepts a function and any number of arguments and returns a new function. Anytime you see a class or a function with documentation stating that one of its arguments should be a callable or a callable object,