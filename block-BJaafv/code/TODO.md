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
```js
    //The first function will return a value that will be a+b and the second function is printing the output of a+b and it will return undefined. 
```
2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
```js

    // The value of first will be a+b and value of second will be undefined
```
3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

```js
      //The output will be 36 the first two argument values will be passed to the parameters and 35 won't be passed to any parameters because there is only two parameters.

```

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

```js
      //yes we can add the sum function as a value to the variable add because in js functions are ojects. Objects are values so we can assign a function to variable.  

```

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js

   function sayHello(name) {
     name =`Hello Arya`;
     return name;
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
````js
      //Here the output will "Hello John" because inside the function  we are defining a userName variable so the function will outside for the variable .

```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1 //The output will be "John"

showMessage(); // Output 2 //"Hello, John"

alert(userName); // Output 3 //"John"
```

8. What is a Anonymous Function give example of three functions.

```js
      //Anonymous functions arelike function expressions without function name

      eg:- let add = function(num1, num2) {
        return num1+num2;
      }

      //Arrow functions are the short form of anonymous functions without function keyword

      eg:- let add = (num1, num2) => {
        return num + num2;
      }

      //function expressions are like we are assigning a function to a variable and we will call the function using variable name

      eg:- let add = function addNum(num1, num2) {
        return num1 + num2;
      }

```

9. Can function declaration be a Anonymous Function? Explain

```js
      //function declaration cannot become a anonymous function. In function declaration we are using function and we use function names to call the function. In anonymous function we don't use function names and we call the function using variable name.


```

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

// function showValues(){

}

function getData() {

}

function calculateArea() {

}

function createVariables() {

}

function getInput() {
  
}