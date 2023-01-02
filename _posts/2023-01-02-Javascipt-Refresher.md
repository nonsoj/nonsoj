---
layout: post
title: "Javascript Refresher"
date: 2023-01-02
categories: Post
---

#### Rough Unorganized Notes

---

---

- `data types` include :
- Numbers; decimal numbers, integers, negative numbers, non-negative numbers, (can you use complex numbers in javascript code?)
- strings - single `' '` or double quotes `" "`
- using quotes tell javascript to execute the input as a string
- string concatenation
- how scripts in javascript get executed
- from top to bottom
- you can initilize the value of another variable or another constant in a newly assigned variable
- always be consistent when using quotes
- string operations
- using single or double quotes as string delimiters
- backticks
- `${ }` --> tells js to execute the expression in the template literal and only works with backticks
- template literals can be used to write multi-line strings
- helps with text readability
- span expressions over multiple lines
- `\n` newline operator (line break)
- mixing single and double quotes to concatenate strings
- `\` --> ignore the next character
- \\ execute the backslash after the backslash
- functions
- language scope
- readablity in code
- built-in functions in the language
- you can run funtions multiple times
- never repeat yourself
- returning functions
- order of code execution
- functions can be placed anywhere in the code body / script because js parses the script and searches for functions before executing code
- variables and expressions on the other hand cannot be called before they are initialized
- global scope and local scope
- you can read constants and variables assigned globally but you can't use variables and constants in a function because they are local variables
- functions can interact with global variables ; variables and constants assigned outside the function body and reassign them for use in the function body --> bad code
- pure functions
- `return` ends the code execution
- you can also return nothing --> `return`;
- declare javascript variables with the var keyword --> `var Nonso`;
- A string literal, or string, is a series of zero or more characters enclosed in single or double quotes
- When JavaScript variables are declared, they have an initial value of `undefined`. If you do a mathematical operation on an `undefined` variable your result will be `NaN` which means "Not a Number". If you concatenate a string with an `undefined` variable, you will get a string of `undefined`
- uninitialized variables and how javascript executes them in code
- In JavaScript all variables and function names are case sensitive. This means that capitalization matters
- Write variable names in JavaScript in camelCase. In camelCase, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.
- variables declared using `const` are read-only
- It is common for developers to use uppercase variable identifiers for immutable values and lowercase or camelCase for mutable values (objects and arrays)
- increment and decrement values in javascript with the `++` or `--` operator. -->
  `firstValue = 15;`
  `firstValue++ //increments firstValue by 1`
  `secondValue = -15;`
  `secondValue-- //-16 decreases secondValue by 1`
- Decimal numbers are sometimes referred to as `floating point` numbers or `floats`.
- The remainder operator `%` gives the remainder of the division of two numbers
- In programming, it is common to use assignments to modify the contents of a variable. Remember that everything to the right of the equals sign is evaluated first, so we can say
- In JavaScript, you can escape a quote from considering it as an end of string quote by placing a backslash (`\`) in front of the quote.
- CodeOutput`\'`single quote`\"`double quote`\\`backslash`\n`newline`\t`tab`\r`carriage return`\b`word boundary`\f`form feed
- Solution --> `const myStr = "FirstLine\n\t\\SecondLine\n\ThirdLine"`;
- Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself
- We can also use the `+=` operator to concatenate a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines
- --> ``js
let ourStr = "I come first. ";
ourStr += "I come second.";
`
- Just as we can build a string over multiple lines out of string literals, we can also append variables to a string using the plus equals (`+=`) operator.

Example:

```js
const anAdjective = "awesome!";
let ourStr = "freeCodeCamp is ";
ourStr += anAdjective;
```

`ourStr` would have the value `freeCodeCamp is awesome!`

- string operations in javascript
- you can find the length of a `String` value by writing `.length` after the string variable or string literal
- Bracket notation is a way to get a character at a specific index within a string
- Most modern programming languages, like JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as Zero-based indexing.

For example, the character at index 0 in the word `Charles` is `C`. So if `const firstName = "Charles"`, you can get the value of the first letter of the string by using `firstName[0]`

- `firstName[0]` --> square brackets not `( ) or { }`
- In JavaScript, `String` values are immutable, which means that they cannot be altered once created

- You can also use bracket notation to get the character at other positions within a string.

Remember that computers start counting at `0`, so the first character is actually the zeroth character

- In order to get the last letter of a string, you can subtract one from the string's length.
- For example, if `const firstName = "Ada"`, you can get the value of the last letter of the string by using `firstName[firstName.length - 1]`
- multi-dimensional arrays
- We can access the data inside arrays using indexes
- Unlike strings, the entries of arrays are mutable and can be changed freely, even if the array was declared with `const`
- An easy way to append data to the end of an array is via the `push()` function
- `.push( )` appends any new variable/parameters to the end of the array
- converting strings to numbers using parseInt function or + sign
- the function position in the script doesn't matter
- `.pop()` is used to pop a value off of the end of an array
- Any type of entry can be popped off of an array - numbers, strings, even nested arrays
- `pop()` always removes the last element of an array. What if you want to remove the first?

That's where `.shift()` comes in. It works just like `.pop()`, except it removes the first element instead of the last

- `Parameters` are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input (or "passed") into a function when it is called are known as arguments
- queues --> In Computer Science a queue is an abstract Data Structure where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.
- always break down problems to tiiny chunks and solve from there
- `//` this is a comment
- `/* this is also a (multi-line) comment */`
- how to use comments --> do not comment the obvious
- make comments brief and avoid writing daunting comments
- `+= or -+ or /= or \*=` --> shortcut operators in javascript
- more datatypes --> `booleans` ; `true / false`
  - objects `{
`key-value pairs:} i.e grouped or related data`    -`arrays [ data] [ lists ] ?`
- Booleans may only be one of two values: `true` or `false`. They are basically little on-off switches, where `true` is on and `false` is off. These two states are mutually exclusive.
- Boolean values are never written with quotes. The strings `"true"` and `"false"` are not Boolean and have no special meaning in JavaScript.
- conditional operators in javascript
  - [Conditional Operators](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-conditional-logic-with-if-statements)
- the equality operator --> The most basic operator is the equality operator `==`. The equality operator compares two values and returns `true` if they're equivalent or `false` if they are not. Note that equality is different from assignment (`=`), which assigns the value on the right of the operator to a variable on the left.
- Strict equality (`===`) is the counterpart to the equality operator (`==`). However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.

If the values being compared have different types, they are considered unequal, and the strict equality operator will return false.

- type of operator --> `typeof`
- The inequality operator (`!=`) is the opposite of the equality operator. It means not equal and returns `false` where equality would return `true` and *vice versa*. Like the equality operator, the inequality operator will convert data types of values while comparing.
- The strict inequality operator (`!==`) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns `false` where strict equality would return `true` and *vice versa*. The strict inequality operator will not convert data types.
- The greater than operator (`>`) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns `true`. Otherwise, it returns `false`
- The greater than or equal to operator (`>=`) compares the values of two numbers. If the number to the left is greater than or equal to the number to the right, it returns `true`. Otherwise, it returns `false`
- The less than operator (`<`) compares the values of two numbers. If the number to the left is less than the number to the right, it returns `true`. Otherwise, it returns `false`. Like the equality operator, the less than operator converts data types while comparing
- The less than or equal to operator (`<=`) compares the values of two numbers. If the number to the left is less than or equal to the number to the right, it returns `true`. If the number on the left is greater than the number on the right, it returns `false`. Like the equality operator, the less than or equal to operator converts data types
- Sometimes you will need to test more than one thing at a time. The logical and operator (`&&`) returns `true` if and only if the operands to the left and right of it are true
- The logical or operator (`||`) returns `true` if either of the operands is `true`. Otherwise, it returns `false`
- js objects -->  
   ` const object` = `{
`name: 'string'`,
`age: int`,
`department: field-of-study`,
`hobbies: array[list]`,
`property: function(),` 
}`

- accessing objects using dot notation e.g `console.log(object.property)`

-
