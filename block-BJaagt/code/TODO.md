Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); //In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The declaration of the variable is block scoped and we can't access the variable defined inside a block from outside.
```

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The declaration of the variable is block scoped and we can't access the variable defined inside a block from outside.
```

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); //In above code we are looking for the variable named `username`. We will get Arya as a result because var is only functional scoped, so we can access the value of username from  a block scope.
```

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); //In above code we are looking for the variable named `username`. We are getting error because  var is only functional scoped and because of hoisting var decalration will be move to  the top and after that we are  trying to redeclare the variable with same name using let.
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); //In the above code we are looking for a varibale username. the value of username is "John" because let is block scoped so if try to access the varible outside the scope we will get error, but the value username is also declare outside the global scope, so we can access its value.

```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); //In the above code we are looking for a varibale username. the value of username is "John" because let is block scoped so if try to access the varible outside the scope we will get error, but the value username is also declare outside the global scope, so we can access its value.
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); //Because var will create a  global scope , so when the loop will run,it will give the value from 0 to 10 inside the block scope, after that loop will be terminated and the value i will be 10 and after that second console log will be executed and it will give 10.
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); //beacuse i is not defined.
```

