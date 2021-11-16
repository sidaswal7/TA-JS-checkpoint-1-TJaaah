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
// First function returns the sum of both the values and the second function logs their sum in the console.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
2. Value of `first` will be sum of a and b. And value of second will be undefined.
3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
3. It will throw an error because the function only has to parameters so it cant take 3 arguments.
4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
4. Yes we can store the first `sum` function and it is called function expression
5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name){
  return `Hello ${name}`;
}
6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
// 'Hello John' will be the output because username="john" is defined outside the function, so it will look for username variable outside the function.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // 'john'

showMessage(); // 'hello john'

alert(userName); // 'john'
```

8. What is a Anonymous Function give example of three functions.
8. The function without name is called anonymous function.
  eg1: let userName= (a)=> `hello ${a}`;
  eg2: let addSum= (a,b)=> a+b;
  eg3: let squareNum= (n)=> n*n;
9. Can function declaration be a Anonymous Function? Explain
9. Yes, function declaration can be anonymous.
  eg: ```js
    function add(a,b){
      return a+b;
    }
  can also be written as:
  let add= (a,b)=> a+b;  
10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.
10. - Name of the function should be a verb as they are made to carry out actions.
    - Name should also be brief and describe the action it has to carry out.
    - Avoid generic name
    eg: function addNumbers(a,b){
      return a+b;
    };
    This function name is addNumbers because it takes two input and return their sum.
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
