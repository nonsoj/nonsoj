---
layout: post
title: "Javascript refresher contd"
date: 2023-01-04
categories: Post
---

##### Personal (rough) unorganized notes

---

- selecting from many options with switch statement --> If you have many options to choose from, use a switch statement. A `switch` statement tests a value and can have many case statements which define various possible values. Statements are executed from the first matched `case` value until a `break` is encountered
- ```js
  switch (lowercaseLetter) {
    case "a":
      console.log("A");
      break;
    case "b":
      console.log("B");
      break;
  }
  ``;
  ```

- objects can also be accessed using bracket notation `([])`
- Dot notation is what you use when you know the name of the property you're trying to access ahead of time
- ```js
  const myObj = {
    prop1: "val1",
    prop2: "val2",
  };
  ```

const prop1val = myObj.prop1;
const prop2val = myObj.prop2;
``

- If the property of the object you are trying to access has a space in its name, you will need to use bracket notation. However, you can still use bracket notation on object properties without spaces
- ```js
  const myObj = {
    "Space Name": "Kirk",
    "More Space": "Spock",
    NoSpace: "USS Enterprise",
  };
  ```

myObj["Space Name"];
myObj['More Space'];
myObj["NoSpace"];
``

- Note that property names with spaces in them must be in quotes (single or double)
- Another use of bracket notation on objects is to access a property which is stored as the value of a variable. This can be very useful for iterating through an object's properties or when accessing a lookup table.
- Here is an example of using a variable to access a property:

```js
const dogs = {
  Fido: "Mutt",
  Hunter: "Doberman",
  Snoopie: "Beagle",
};

const myDog = "Hunter";
const myBreed = dogs[myDog];
console.log(myBreed);
```

- use quotes when appending new object properties and also when accessing object properties with bracket notation
- use the `delete` keyword to delete object properties for example:
- ```js
  delete myObject.property name / delete myObject['property-name'];
  ```

  - accessing nested objects :

- The sub-properties of objects can be accessed by chaining together the dot or bracket notation.
- You can run the same code multiple times by using a loop.

The first type of loop we will learn is called a `while` loop because it runs while a specified condition is true and stops once that condition is no longer true

- You can run the same code multiple times by using a loop.

The most common type of JavaScript loop is called a `for` loop because it runs for a specific number of times.

For loops are declared with three optional expressions separated by semicolons:

`for (a; b; c)`, where `a` is the initialization statement, `b` is the condition statement, and `c` is the final expression.

The initialization statement is executed one time only before the loop starts. It is typically used to define and setup your loop variable.

The condition statement is evaluated at the beginning of every loop iteration and will continue as long as it evaluates to `true`. When the condition is `false` at the start of the iteration, the loop will stop executing. This means if the condition starts as false, your loop will never execute.

The final expression is executed at the end of each loop iteration, prior to the next condition check and is usually used to increment or decrement your loop counter.

In the following example we initialize with `i = 0` and iterate while our condition `i < 5` is true. We'll increment `i` by `1` in each loop iteration with `i++` as our final expression.

- A common task in JavaScript is to iterate through the contents of an array. One way to do that is with a `for` loop. This code will output each element of the array `arr` to the console
- If you have a multi-dimensional array, you can use the same logic as the prior waypoint to loop through both the array and any sub-arrays. Here is an example:
- ```js
  const arr = [
    [1, 2],
    [3, 4],
    [5, 6],
  ];
  ```

for (let i = 0; i < arr.length; i++) {
for (let j = 0; j < arr[i].length; j++) {
console.log(arr[i][j]);
}
}

- The next type of loop you will learn is called a `do...while` loop. It is called a `do...while` loop because it will first `do` one pass of the code inside the loop no matter what, and then continue to run the loop `while` the specified condition evaluates to `true`
- Recursion is the concept that a function can be expressed in terms of itself
