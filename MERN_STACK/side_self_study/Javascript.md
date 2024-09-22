# Study Guide: Basic JavaScript Syntax

## Introduction

JavaScript is a versatile programming language widely used for web development. It allows developers to create interactive web applications and manipulate web page content dynamically. This guide provides an overview of basic JavaScript syntax to help you practice and understand its core concepts.

## Basic Concepts

### 1. Variables
Variables are used to store data values, allowing you to reference and manipulate that data throughout your code.

- **Declaration**: Use `var`, `let`, or `const` to declare a variable.
  
  - **`var`**: Declares a variable that can be re-assigned. It's function-scoped or globally-scoped.
  - **`let`**: Declares a block-scoped variable, allowing for re-assignment.
  - **`const`**: Declares a block-scoped variable that cannot be re-assigned (must be initialized at declaration).

  ```javascript
  var name = "Henry"; // Older syntax, function-scoped
  let age = 27;       // Block-scoped
  const PI = 3.14;   // Constant value, cannot be changed
  ```

### 2. Data Types
JavaScript has several data types that help define the kind of data you can work with:

- **String**: A sequence of characters enclosed in quotes.
- **Number**: Numeric values, both integers and floating-point numbers.
- **Boolean**: Represents a value that can either be `true` or `false`.
- **Array**: An ordered list of values, which can be of mixed types.
- **Object**: A collection of key-value pairs.

Example:
```javascript
let fruits = ["apple", "banana", "cherry"]; // Array of strings
let person = { name: "Henry", age: 27 };    // Object with properties
```

### 3. Operators
Operators are used to perform operations on variables and values, allowing for various calculations and comparisons.

- **Arithmetic Operators**: Used for mathematical operations.
  
  ```javascript
  let sum = 10 + 5;  // Addition results in 15
  let product = 10 * 5; // Multiplication results in 50
  ```

- **Comparison Operators**: Used to compare two values. The result is always a boolean (`true` or `false`).

  ```javascript
  let isEqual = (5 === 5); // Strict equality check; true
  let isNotEqual = (5 !== 4); // true
  ```

- **Logical Operators**: Used to combine boolean values.

  ```javascript
  let isAdult = (age >= 18 && age < 65); // true if age is between 18 and 64
  ```

### 4. Control Structures
Control structures help manage the flow of execution in your code.

- **Conditional Statements**: Execute different blocks of code based on certain conditions.

  ```javascript
  if (age >= 18) {
      console.log("Adult");
  } else {
      console.log("Minor");
  }
  ```

- **Loops**: Allow code to be executed repeatedly based on a condition.

  ```javascript
  for (let i = 0; i < 5; i++) {
      console.log("Count: " + i); // Outputs 0 to 4
  }
  ```

### 5. Functions
Functions are reusable blocks of code that perform a specific task. They can take inputs (parameters) and return outputs.

- **Function Declaration**:

  ```javascript
  function greet(name) {
      return "Hello, " + name + "!";
  }
  console.log(greet("Alice")); // Outputs: Hello, Alice!
  ```

- **Function Expression**: A function can also be defined and assigned to a variable.

  ```javascript
  const add = function(a, b) {
      return a + b;
  };
  console.log(add(5, 3)); // Outputs: 8
  ```

- **Arrow Functions** (ES6): A more concise way to write functions.

  ```javascript
  const multiply = (a, b) => a * b;
  console.log(multiply(4, 5)); // Outputs: 20
  ```

### 6. Events
JavaScript can respond to user interactions through events, allowing for dynamic user experiences.

```javascript
document.getElementById("myButton").addEventListener("click", function() {
    alert("Button clicked!"); // Displays an alert when the button is clicked
});
```

This code attaches an event listener to a button with the ID `myButton`, triggering an alert when the button is clicked.

---

## Conclusion

Practicing basic JavaScript syntax is essential for mastering web development. By experimenting with variables, functions, control structures, and events, you can gain a solid understanding of how JavaScript works. The skills you develop through practice will form the foundation for building more complex applications.

## References
- [MDN Web Docs: JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [JavaScript Info](https://javascript.info/)
- [W3Schools: JavaScript Tutorial](https://www.w3schools.com/js/)