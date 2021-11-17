1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let sum = 0;
for(let i=1;i<=10;i++){
  let input = Number(prompt("Enter the value"));
  sum += input;
}
let avg = sum/10;
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
//Error println is not defined

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
 function getEvenSum(max=10){
   let sum = 0;
   for(let i=1;i<=max;i++){
     if(i%2 == 0){
       sum += i;
     }
   }
   return sum;
 }
```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
 function getOddSum(max=10){
   let sum = 0;
   for(let i=1;i<=max;i++){
     if(i%2 == 1){
       sum += i;
     }
   }
   return sum;
 }
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
```js
function getProductOfDigits(num){
        if(num == 0){
          return `Not a valid input`;
        } else {
          let prod = 1;
          while(num!=0){
            prod = prod*(num%10);
            num = Math.floor(num / 10);
          }
          return prod;
        }
      }
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // Bigger than 5
check(1); // Smaller than 5
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'
getOutput('John'); // 'You are john'
getOutput(); // 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'Who are you'
getOutput('John'); // 'Who are you'
getOutput(); // 'Who are you'
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
9. A function can have multiple return statements but only one can be executed based on the condition.
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
10. The difference between for loop and while loop is that in for loop the number of iterations to be done is already known whereas in while loop the commands run until a certain condition is reached.