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
