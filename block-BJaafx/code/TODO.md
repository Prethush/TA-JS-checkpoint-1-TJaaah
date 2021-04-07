1. Using loops take 10 inputs from user and find the average of all the numbers.

let sum = 0;
for(let i = 0; i < 10; i++) {
  let num = +prompt("Enter the number");
  sum += num;
}

let average = sum / 10;

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
//the output is println is not defined

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

let sum = 0;
function getEvenSum(max = 10) {
    for(let i = 1; i <= max; i++) {
      if(i % 2 === 0) {
      sum += i;
    }
    }
    return sum;
}

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

function getOddSum(max = 10) {
  for(let i = 1; i <= max; i++) {
      if(i % 2 !== 0) {
      sum += i;
    }
    }
    return sum;
}
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

function getProductOfDigits(num) {
  let product = 1, str = String(num);
  for(let i = 0; i < str.length; i++) {
    product *= Number(str[i]);
      
  }
  return product;
}

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

check(10); // "Bigger than 5"
check(1); // "Smaller than 5"
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // "You are arya" here the value argument is "Arya" it matches with the if condition so it will return statement
getOutput('John'); // "You are john" here the value argument is "John" it matches with the if condition so it will return statement
getOutput(); // "Who are you" here we are not passing any arguments so it return the last return statement
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); //"You are arya" here the value argument is "Arya" it matches with the if condition so it will return statement
getOutput('John'); // "You are john" here the value argument is "John" it matches with the if condition so it will return statement
getOutput(); // "Who are you" here we are not passing any arguments so it return the last return statement
```
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
A function cannot have multiple return statements. If we add more than one return statement after execting the first return statement the flow of the program will come oustide the function.
     eg:- function add(num1, num2) {
       return num1 + num2;
       return `Sum = ${num1} + ${num2}`; //these return statement won't get executed
     }

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

Diffrence between for loop and while loop is that inside the for loop we are creating the loop variable and assigning the value for it. There are 3 sections in the for loop initialization , condition and the iteration part. In while loop we create the loop variable outside the loop. We will only check the condition in the loop section and the iteration part will inside the body of the loop. If we aleady know how many times our loop will excute then for loop is the best or if we don't know how many times our loop will execute then while loop is the option. We use loops to repeat a task muliple times.

eg:- for(let i = 0; i < 10; i++) {
  console.log("Hello World!");
}

let i = 0;
while(i < 10) {
  console.log("Hello World");
  i++;
}



