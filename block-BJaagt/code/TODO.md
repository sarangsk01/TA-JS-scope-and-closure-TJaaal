Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output  Uncaught ReferenceError: username is not defined
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // output Uncaught ReferenceError: username is not defined
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the variable defined inside a block from outside because its function scoped.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output Uncaught ReferenceError: username is not defined
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the statement and we can't access the variable defined inside a statement from outside.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // output Arya
```
In above code we are looking for the variable named `username`.The variable is inside the statement defined with var therefore we can access the variable from outside because var only function scoped.

The above code will throw an error `Reference Error username is not defined`.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output Uncaught SyntaxError: Identifier 'username' has already been declared
```
In above code we are looking for the variable named `username`.The variable is already declared on global scope and after that it declared inside the statement defined with var therefore it will throw an error.

The above code will throw an error `SyntaxError: Identifier 'username' has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output Uncaught SyntaxError: Identifier 'username' has already been declared
```
In above code we are looking for the variable named `username`.The variable is already declared on global scope and after that it declared inside the statement defined with let therefore it will throw an error because variable defined with let will not overwritten the value with let.

The above code will throw an error `SyntaxError: Identifier 'username' has already been declared`.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output Uncaught SyntaxError: Identifier 'username' has already been declared
```
In above code we are looking for the variable named `username`.The variable is already declared on global scope and after that it declared inside the function defined with let therefore it will throw an error because variable defined with let will not overwritten the value with let.

The above code will throw an error `SyntaxError: Identifier 'username' has already been declared`.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
0 'First'
1 'First'
2 'First'
3 'First'
4 'First'
5 'First'
6 'First'
7 'First'
8 'First'
9 'First'
}
console.log(i, 'Second'); // output 10 'Second'
```
In above code we are looking for the value of i.i is defined with var keyword its not statement scoped.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
0 'First'
1 'First'
2 'First'
3 'First'
4 'First'
5 'First'
6 'First'
7 'First'
8 'First'
9 'First'
}
console.log(i, 'Second'); // output 10 'Second'
```
In above code we are looking for the value of i.i is defined with let keyword its not statement scoped.
```
