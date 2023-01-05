---
layout: post
title: "Javascript refresher contd"
date: 2023-01-02
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
