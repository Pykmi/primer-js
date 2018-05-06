# Javascript Primer
## Variables
All off programming can be defined as the manipulation of information. For this purpose, in programming we use variables to store data and we use different data types for different types of information.

Declaring new variables are done by using the correct keyword and the name of the variable. Optionally, you can also assign the variable with a value.

In Javascript, what we call primitive types, are Number, String, Boolean, Null, and Undefined.

```javascript
// numbers include both decimals and whole number
var pi = 3.14;
var ten = 10;

// strings are any series of characters, like words and sentences
var mice = "Three blind mice. See how they run.";

// booleans only have true or false values
var yes = true;
var no = false;

// null means empty of value, a data type for when our variable does not have a value
var empty = null;
```

### Keywords
Most common keyword for declaring a variable in Javascript is `var`, however since ES6 Javascript also recognises two other keywords as well; `let` and `const`.

The difference between var and let is particularly confusing many; the main difference being `scope`.

```javascript
// var is scoped to the nearest function
var pi = 3.14;

// let is scoped to the nearest enclosing block
let euler = 2.718;

// const defines an immutable variable
const ten = 10;
ten = 10.0; // SyntaxError: Assignment to constant variable
```

### Let vs. Var
The difference between the two is scope, whereas var scopes the variable to the nearest function, let scopes the variable to the nearest enclosed block.

```javascript
// example for the behaviour of var
function varExample() {
	// 'i' is visible here

	for(var i = 0; i < 7; i++) {
	  // 'i' is visible here
	}

	// 'i' is visible here
}
```

```javascript
// example for the behaviour of let
function letExample() {
	// 'e' is NOT visible here

	for(var e = 0; i < 7; i++) {
	  // 'e' is visible here
	}

	// 'e' is NOT visible here
}
```

