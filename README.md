JavaScript is a high-level, multi-paradigm programming language primarily used for website development alongside HTML and CSS. While HTML and CSS provide the structure and style of a website, JavaScript enables the addition of interactive features and behaviors. This allows visitors to engage with the website in more exciting ways. Also note that the language is not limited to a specific type of operating system and supports event-driven, functional, and imperative programming styles such as object-oriented and prototype-based. 

JavaScript has gained immense popularity since its release in 1995. According to Statista, 65% of developers are using JavaScript worldwide today, and it surpassed other languages such as Java and Python. What makes JavaScript so developer-friendly is the fact that it’s relatively easy to learn and allows developers to rapidly build apps with massive audiences.

You can use JavaScript to create:

Web applications, servers and backend web infrastructure;
Browser-based games;
Animation and other special effects;
Security features (such as passwords);
Automatically refreshing news feeds;
Mobile applications.
Like all languages, JavaScript is constantly changing. Here’s a brief overview of JavaScript’s version history and how this programming language has evolved

JavaScript is a modern scripting language that is popular worldwide among developers. It is a lightweight, interpreted compiled language that can be used on both client-side as well as the server side. It was invented in the year 1995 by Brendan Eich. Over the years the language has improved a lot and a lot of new features have been added which make the coding process even easier. This language became an ECMA standard in the year 1997.

n JavaScript, variables and constants are used to store data values. Here's an overview of both:

Variables:
A variable is a container for storing data values. You can think of a variable as a named storage location for data that can be changed during the execution of a program. To declare a variable in JavaScript, you use the var, let, or const keyword.

A constant is like a variable, but its value cannot be changed once it is defined. In JavaScript, constants are declared using the const keyword.
Use var for variables that need function-level scope (or global if needed), but prefer let for block-level scope.
Use const for values that should not be re-assigned.
Constants should be used when you know the value shouldn't change during the execution of your program.
Remember, using let and const was introduced in ES6 (ECMAScript 2015) and is more modern and recommended over using var, especially for variables. Use const by default for values that should not be reassigned, and use let for values that you expect to change.

Javascript has seven primitive data types:

string
number
bigint
boolean
undefined
symbol
null
In JavaScript, a primitive is any value that isn't an object.

The typeof operator tells you what type a primitive value is.

String
It is important to note that strings can be either a primitive, string literal, or an object. Javascript automatically converts string primitives to objects to enable the user to use the handy array of functions available for use. If you wanted to convert a string object to a primitive, you would use the valueOf() method.

let message = "Hello World";
typeof message; // 'string'
Number
In other programming languages, you can have numbers be defined as floats, integers, doubles and so on and so forth. Javascript simplified this feature by just making every number it comes across Number, with an exception.

let password = 123456789;
typeof password; // 'number'
BigInt
This is similar to Number however, it allows you to safely represent integer values larger than 253. You can create a bigint by appending n to the end of the number or by wrapping the number, or string for this case, in the BigInt() constructor.

let launchCodes = 66777888889999912345n;
typeof launchCodes; // 'bigint'
Boolean
This data type is what contains the values true or false. This is great in that you can use other values to represent that same concept like 0 for false, and 1 for true.

isBool = true;
typeof isBool; // 'boolean'

// Instances of wrapper classes, like `Boolean`, are objects, **not** primitives.
typeof new Boolean(isBool); // 'object'
Undefined
This value is automatically assigned to variables that have just been declared but not defined. If you were to put this in an if statement, the value would be false so this is another handy thing you could use like mentioned in the Boolean section.

let x;

typeof x; // 'undefined'
Symbol
A Symbol is a value created by invoking the Symbol function which is guaranteed to create a unique value. It takes one parameter, a string description, that will show up when you print the symbol.

let x = Symbol("this is a symbol");
typeof x; // 'symbol'
Null
null is special because the typeof operator reports its type as 'object'.

typeof null; // 'object'

There are following types of operators in JavaScript.

Arithmetic Operators
Comparison (Relational) Operators
Bitwise Operators
Logical Operators
Assignment Operators
Special Operators
JavaScript Arithmetic Operators
Arithmetic operators are used to perform arithmetic operations on the operands. The following operators are known as JavaScript arithmetic operators.
ADVERTISEMENT


Operator	Description	Example
+	Addition	10+20 = 30
-	Subtraction	20-10 = 10
*	Multiplication	10*20 = 200
/	Division	20/10 = 2
%	Modulus (Remainder)	20%10 = 0
++	Increment	var a=10; a++; Now a = 11
--	Decrement	var a=10; a--; Now a = 9

  JavaScript Comparison Operators
The JavaScript comparison operator compares the two operands. The comparison operators are as follows:

Operator	Description	Example
==	Is equal to	10==20 = false
===	Identical (equal and of same type)	10==20 = false
!=	Not equal to	10!=20 = true
!==	Not Identical	20!==20 = false
>	Greater than	20>10 = true
>=	Greater than or equal to	20>=10 = true
<	Less than	20<10 = false
<=	Less than or equal to	20<=10 = false

Conditional statements in JavaScript allow you to execute specific blocks of code based on conditions. If the condition meets then a particular block of action will be executed otherwise it will execute another block of action that satisfies that particular condition.

There are several methods that can be used to perform Conditional Statements in JavaScript.

if Statement
if-else Statement
else if Statement
switch Statement
Ternary Operator
We will explore all the above methods along with their basic implementation with the help of examples.

JavaScript if Statement
The if statement is used to evaluate a particular condition. If the condition holds true, the associated code block is executed.


Syntax:

if ( condition ) {
    // If the condition is met, 
    //code  will get executed.
}
Example: In this example, we are using the if statement to find given number is even or odd.

Javascript
   
let num = 20; 
  
if (num % 2 === 0) { 
    console.log("Given number is even number."); 
} 
  
if (num % 2 !== 0) { 
    console.log("Given number is odd number."); 
};

Output
Given number is even number.
JavaScript if-else Statement
The if-else statement will perform some action for a specific condition. Here we are using the else statement in which the else statement is written after the if statement and it has no condition in their code block.

Syntax:

if (condition1) {
    // Executes when condition1 is true
    if (condition2) {
        // Executes when condition2 is true
    }
}
Example: In this example, we are using the above-explained approach.

Javascript
   
let age = 25; 
  
if (age >= 18) { 
    console.log("You are eligible of driving licence") 
} else { 
    console.log("You are not eligible for driving licence") 
};

Output
you are eligible of driving licence
JavaScript else if Statement
The else if statement in JavaScript allows handling multiple possible conditions and outputs, evaluating more than two options based on whether the conditions are true or false.

Syntax:

if (1st condition) {
    // Code for 1st condition
} else if (2nd condition) {
    // ode for 2nd condition
} else if (3rd condition) {
    // Code for 3rd condition
} else {
    //  ode that will execute if all 
    // above conditions are false
}
Example: In this example, we are using the above-explained approach.

Javascript
   
const num = 0; 
  
if (num > 0) { 
    console.log("Given number is positive."); 
} else if (num < 0) { 
    console.log("Given number is negative."); 
} else { 
    console.log("Given number is zero."); 
};

Output
Given number is zero.
JavaScript Switch Statement (JavaScript Switch Case)
As the number of conditions increases, you can use multiple else-if statements in JavaScript. but when we dealing with many conditions, the switch statement may be a more preferred option.

Syntax:

switch (expression) {
    case value1:
        statement1;
        break;
    case value2:
        statement2;
        break;
    . . .
    case valueN:
        statementN;
        break;
    default:
        statementDefault;
};
Example: In this example, we find a branch name Based on the student’s marks, this switch statement assigns a specific engineering branch to the variable Branch. The output displays the student’s branch name,

Javascript
   
const marks = 85; 
  
let Branch; 
  
switch (true) { 
    case marks >= 90: 
        Branch = "Computer science engineering"; 
        break; 
    case marks >= 80: 
        Branch = "Mechanical engineering"; 
        break; 
    case marks >= 70: 
        Branch = "Chemical engineering"; 
        break; 
    case marks >= 60: 
        Branch = "Electronics and communication"; 
        break; 
    case marks >= 50: 
        Branch = "Civil engineering"; 
        break; 
    default: 
        Branch = "Bio technology"; 
        break; 
} 
  
console.log(`Student Branch name is : ${Branch}`);

Output
Student Branch name is : Mechanical engineering
JavaScript Ternary Operator ( ?: )
The conditional operator, also referred to as the ternary operator (?:), is a shortcut for expressing conditional statements in JavaScript.

Syntax:

condition ? value if true : value if false
Example: In this example, we use the ternary operator to check if the user’s age is 18 or older. It prints eligibility for voting based on the condition.

Javascript
   
let age = 21; 
  
const result = 
    (age >= 18) ? "You are eligible to vote."
        : "You are not eligible to vote."; 
  
console.log(result);

Output
You are eligible to vote.

JavaScript for Loop
A for loop is used when you know how many times you need to repeat a certain block of code. It takes three statements.

Initialization statement
Condition Statement
Increment statement.
Example: This example shows the use of a for loop.

   
for (let i = 0; i < 4; i++) {
 console.log(i);
}

Output
0
1
2
3
JavaScript while Loop
A while loop is used when you don’t know how many times you need to repeat a block of code, but you know the condition that will end the loop.

Example: This example shows the use of a while loop.

   
let i = 0;
while (i < 6) {
  console.log(i);
  i++;
}

Output
0
1
2
3
4
5
JavaScript do-while Loop
A do-while loop is similar to a while loop, but the block of code is executed at least once, even if the condition is false.

Example: This example shows the use of do-while loop.

   
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 6);

Output
0
1
2
3
4
5
JavaScript for-in Loop
A for-in loop is used to loop through the properties of an object.

Example: This example shows the use of for-in loop.

   
const obj = {a: 1, b: 4, c: 7};
 
for (let prop in obj) {
  console.log(prop + ': ' + obj[prop]);
}

Output
a: 1
b: 4
c: 7
JavaScript for-of Loop
A for-of loop is used to loop through the values of an iterable object (such as an array.

Example: This example shows the use of for-of loop.

   
const arr = [1, 2, 3];
 
for (let val of arr) {
  console.log(val);
}

Output
1
2
3
JavaScript forEach loop
A forEach loop is a method on arrays that executes a function for each element in the array.

Example: This example shows the use of forEach loop.

   
const arr = [1, 2, 3];
arr.forEach(val => console.log(val));

Output
1
2
3
JavaScript map Loop
A map loop is a method on arrays that creates a new array by executing a function on each element in the array.

Example: This example shows the use of map loop.

   
const arr = [1, 2, 3];
const newArr = arr.map(val => val * 2);
console.log(newArr);

Output
[ 2, 4, 6 ]
JavaScript is a widely-used programming language that is essential for web development. Its ability to run on both client-side and server-side makes it a versatile tool that has become an essential tool for web developers.

JavaScript is a high-level, interpreted language used on the client side, meaning it runs in the user's web browser. You can use it to create web and mobile applications, browser extensions, and other software.

It is supported by all major web browsers, and it is an essential technology for front-end web development.

Functions are one of the building blocks of JavaScript programming for creating web applications.

You can think of functions as a way to group a set of instructions together and execute them as a single unit.

In this article, we will explore the basics of functions in JavaScript and how you can use them effectively in your code.

Function Syntax
A function is a block of code that performs a specific task. JavaScript functions are basically used to encapsulate logic, making that code more reusable and easier to understand.

The syntax for creating a function in JavaScript is quite simple. Functions can take input in the form of parameters and can return a value or output.

Functions help you organize and structure your code. They also allow for code reuse and make it easier to understand and maintain large codebases.

How to Write a Function in JavaScript
You start by using the keyword "function," followed by the function name and a set of parentheses.

Inside the parentheses, you can specify any input parameters that the function will take in, also known as arguments. The arguments are usually optional.

Next, you include a block of code inside curly braces that defines the instructions the function will execute when it is called.

Here is an example of a basic function that takes in two numbers and returns their sum:

//index.js

function addNumbers(a, b) {
  return a + b;
}
The function above, named "addNumbers," takes in two parameters, a and b. The code inside the function body simply adds these two parameters together and returns the result.

How to Declare a Function in JavaScript
Apart from the regular way of declaring a function as seen above, you can also define functions using function expressions or arrow functions.

The arrow function syntax is a shorthand version of the regular function syntax. Here is the same function as above, but written with an arrow function:

//index.js
const addNumbers = (a, b) => a + b;
In the example above, the function is assigned to the variable addNumbers. The arrow => is used to define the function, and the code inside the curly braces is the body of the function.

Function expressions in JavaScript are similar to regular function declarations. The difference between them is that the function expression is always assigned to a variable. Here is an example of a function expression:

//index.js
let multiplyNumbers = function(a, b) {
    return a * b;
}
In this example, the function is assigned to the variable multiplyNumbers. This variable can be used to call the function, just like a regular function.

How to Use Callback Functions
Functions can also be passed as arguments to other functions, known as callback functions. Here is an example of a callback function being used to log the result of a multiplication operation:

//index.js

function multiplyByTwo(n, callback) {
  var result = n * 2;
  callback(result);
}

function logResult(result) {
  console.log(result);
}

multiplyByTwo(5, logResult); // logs 10
In this example, the multiplyByTwo function takes two arguments: a number and a callback function. The function multiplies the number by 2 and then invokes the callback function, passing the result as an argument. The logResult function is then executed, which logs the result to the console.

How to Use Default Parameters
JavaScript functions also have a feature called default parameters. They allow you to set default values for parameters in case they are not passed when the function is called.

This is helpful in situations where you want to provide a default value for a parameter in case it is not passed. Here is an example:

//index.js

function greet(name = "John Doe") {
    console.log(`Hello, ${name}!`);
}

greet(); // Hello, John Doe!
greet("Jane Smith"); // Hello, Jane Smith
In this example, the greet function takes in a single parameter name, which is set to "John Doe" by default. If the function is called without passing any arguments, it will use the default value "John Doe". But if an argument is passed, it will use that value instead.

How to Use the Constructor Function
JavaScript has a special type of function called a constructor function, which is used to create objects.

You define a constructor function using the keyword "function" followed by a name that starts with an uppercase letter (called using the "new" keyword).

For example, the following code defines a constructor function named "Person" that creates an object with a name and age property:

//index.js

function Person(name, age) {
  this.name = name;
  this.age = age;
}

let person = new Person("John Smith", 30);
console.log(person.name); // Output: "John Smith"
console.log(person.age); 
How to Use Closures
A closure is a function that has access to variables in its parent scope, even after the parent function has returned. This allows for variables to be preserved between function calls, and it is a powerful feature that allows for more advanced programming patterns such as object-oriented programming.

Here's an example of a closure function that creates a counter:

//index.js

function createCounter() {
  let count = 0;
  return function() {
    return count++;
  }
}
const myCounter = createCounter();
console.log(myCounter()); // Output: 0
console.log(myCounter()); /
How to Use Higher-Order Functions
Functions can also be passed as arguments to other functions, which is known as a "higher-order" function. For example:

//index.js

function performOperation(a, b, operation) {
    return operation(a, b);
}

let result = performOperation(5, 10, addNumbers);
console.log(result);  // 15
In this example, the performOperation function takes in three arguments: a, b, and operation.

The operation argument is a function that takes in two arguments and returns a result. In this case, we are passing the addNumbers function as the operation argument, so the result of the performOperation function will be the result of calling the addNumbers function with the arguments a and b.
