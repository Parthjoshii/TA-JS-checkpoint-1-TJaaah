1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
There is no difference between the functions, but the first one is the correct way to right a function. in the second function, console.log can be written below the first function only, instean of defining a new function.
2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
The value of both will be `unefined`.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
The function will execute only the first 2 parameters as they are defined in the function. therefore it will return the sum of the first 2 parameters which are entered. in this case the return value will be `36` as only 12,24 will be considered and the sum of the same will be returned which is 36.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
No we cant store the function in a variable, as it will throw an error. saying that sum is not defined.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name) {
  return `Hello ${name}`
}
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
`Hello, John` will be the output.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // `John`

showMessage(); // `Hello, John`

alert(userName); // `John`
```

8. What is a Anonymous Function give example of three functions.
A function without a name in a function epression is an Anoymous Function.
examples: let x = (a,b) {
  return a + b;
}

const sum = (num1 , num2) {
  return num1 + num2;
}

9. Can function declaration be a Anonymous Function? Explain
No function declaration canot be an Anonymous function because in function declaration we need to declare a function with a name and parameter, but in case of anonymous function we can just enter the parameters as we are defining the function as an expression.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
function CalcSum(a,b) {
  return a + b;
}

function getName(name) {
  return `Hello ${name};
}

function isAdult(age) {
  return `You're good to go`;
}

function checkIncome(salary) {
  return `Above average`;
}

function createUser(name,age,gender) {
  return `Profile Created`;
}