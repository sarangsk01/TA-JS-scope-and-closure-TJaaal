1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

//
  let percentage = function (marks,total){
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// 
  let percentage = function percentage(marks,total){
  return (marks * 100) / total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```
function percentage(marks, total) {
  return (marks * 100) / total;
}
```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```
function percentage(marks, total) {
  return (marks * 100) / total;
}
```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```
function percentage(marks, total) {
  return (marks * 100) / total;
}
```js
let percentage = (marks, total) => (marks * 100) / total;

function percentage(marks, total) {
  return (marks * 100) / total;
}
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
Ans : when we define a function it is an expression because when executes this function it will get a value.
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
4. Why is a function call an expression in JavaScript?
Ans : A function call is used to execute the function therefore it is also an expression.
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer 5 because we call the function and store it in a variable five.
five = add; // Answer ƒ add(a, b) { return a + b;} it is an function declaration.
five = five(10, 11); // Answer 21 because it will add those two numbers.
five = function () {
  return 'Hello';
}; // Answer     ƒ () {  return 'Hello';} it is an function declaration.
```

6. What is the difference between function definition and function call? Explain with an example.
Ans : The function definition specifies the function name, return type; parameters include a function body.while function call is using this function to achieve the results.
7. What is the similarities between function definition and function call?
Ans : function name is similar in those function definition and function call.
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid valid because it will add properties to the function.
```

9. What is higher order function explain with an example.
Ans : A function that accept function defination with argument or return a function defination from the function is called higher order function.
example : 
let numbers = [1,3,4,8,7];

let isOdd = function(num){
  return num % 2  !==0; 
}
// higher order function
function filterOdd(arr){
  let finalArray = [];
  for(let num of arr){
    if(isOdd(num)){
      finalArray.push(num);
    }
  }
}

10. Explain what is callback function. Why you can pass a function inside a function?
Ans : For example when we define a function filter it accept two parameter arr and cb which will find odd number add return a new array with odd Numbers.Then it is necessary to define callback function of oddNumber to this function to find the value.