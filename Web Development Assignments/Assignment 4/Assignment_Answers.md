# Q.1 Explain Hoisting in JavaScript

Ans: Hoisting in JavaScript is a behavior where variable and function declarations are moved to the top of their scope during compilation. Variables declared with `var` are hoisted but remain undefined until assigned a value. Function declarations are fully hoisted, allowing them to be called before their actual declaration. Block-scoped variables declared with `let` and `const` are hoisted to the top of their block but are not initialized, leading to a "temporal dead zone" if accessed before the declaration.

# Q.2 Explain Temporal Dead Zone?

Ans: The Temporal Dead Zone (TDZ) is a period in JavaScript where variables declared with `let` and `const` exist but cannot be accessed until their actual declaration. Accessing these variables during the TDZ results in a ReferenceError. It helps catch potential errors and encourages proper variable declaration before usage.

# Q.3 Difference between var & let?

Ans: The main differences between `var` and `let` in JavaScript are as follows:

1. Scope: Variables declared with `var` are function-scoped, meaning they are accessible throughout the entire function in which they are defined. On the other hand, variables declared with `let` are block-scoped, meaning they are limited to the block in which they are defined (e.g., within curly braces {}).

2. Hoisting: Variables declared with `var` are hoisted to the top of their scope during compilation, allowing them to be accessed before their actual declaration. `let` variables are also hoisted, but they remain in the Temporal Dead Zone (TDZ) until their actual declaration, and accessing them before declaration results in a ReferenceError.

3. Redeclaration: Variables declared with `var` can be redeclared within the same scope without any error. This can lead to unexpected behavior and potential bugs. `let` variables, on the other hand, cannot be redeclared within the same block scope. Attempting to redeclare a `let` variable will result in a SyntaxError.

4. Global Scope: Variables declared with `var` outside of any function become properties of the global object (e.g., `window` object in a browser). This can inadvertently create or modify global variables, leading to potential conflicts. `let` variables declared outside of a block scope do not become properties of the global object, mitigating such risks.

# Q.4 What are the major features introduced in ECMAScript 6?

Ans: Some major features introduced in ECMAScript 6 (ES6) include block-scoped declarations (`let` and `const`), arrow functions, classes, template literals, destructuring assignment, default parameters, rest and spread operators, modules, promises, and iterators/generators. These features improve scoping control, provide syntactic enhancements, simplify asynchronous programming, and enhance code organization and maintainability.

# Q.5 What is the difference between let and const ?

Ans: The main difference between `let` and `const` in JavaScript lies in their reassignability and mutability:

1. Reassignability:
   - Variables declared with `let` can be reassigned to a new value. This means you can assign a different value to the same variable later in your code.
   - Variables declared with `const`, on the other hand, cannot be reassigned after they are initialized. Once a `const` variable is assigned a value, it remains constant throughout the execution of the program.

2. Mutability:
   - `let` variables are mutable, meaning their value can be changed.
   - `const` variables are considered immutable in the sense that their binding (the reference to a value) cannot be changed. However, the value itself can still be mutable if it is an object or an array. This means you can modify the properties or elements of the object or array assigned to a `const` variable.

To summarize:
- `let` allows reassignment and is mutable.
- `const` does not allow reassignment after initialization and is immutable regarding the variable's binding. However, if the value assigned to a `const` variable is an object or array, its properties or elements can still be modified.

It's worth noting that both `let` and `const` provide block scoping, meaning they are limited to the block in which they are defined. This ensures better control over variable visibility and prevents potential issues caused by variable hoisting.

# Q.6  What is template literals in ES6 and how do you use them?

Ans: Template literals in ES6 are a way to work with strings in JavaScript. They are denoted by backticks (`) and allow for string interpolation, multiline strings, and embedding expressions using `${expression}` syntax. They provide a concise and readable way to create dynamic strings and templates.

# Q.7 What’s difference between map & forEach?

Ans: The main differences between `map` and `forEach` are:

1. Return Value:
   - `forEach` does not return a value. It performs an operation on each element of an array.
   - `map` returns a new array with the results of the callback function applied to each element.

2. Creating a New Array:
   - `forEach` does not create a new array. It simply iterates over the array and executes the provided callback function on each element.
   - `map` creates a new array by applying the provided callback function to each element and collecting the returned values.

3. Usage:
   - Use `forEach` when you want to perform an operation or action on each element of an array.
   - Use `map` when you want to transform an array by applying a function to each element and collecting the results in a new array.

It's important to note that neither `forEach` nor `map` modify the original array directly. However, the callback functions passed to them can modify individual elements of the original array.

# Q.8 How can you destructure objects and arrays in ES6?

Ans: To destructure objects and arrays in ES6, you can use the following syntax:

1. Object Destructuring:
   - To extract values from an object, you can destructure it by matching the variable names with the object's property names.

   ```javascript
   const person = { name: 'John', age: 30 };

   const { name, age } = person;
   console.log(name); // Output: John
   console.log(age); // Output: 30
   ```

2. Array Destructuring:
   - To extract values from an array, you can destructure it by using square brackets `[]` and assigning variables to the corresponding array elements.

   ```javascript
   const numbers = [1, 2, 3];

   const [firstNumber, secondNumber, thirdNumber] = numbers;
   console.log(firstNumber); // Output: 1
   console.log(secondNumber); // Output: 2
   console.log(thirdNumber); // Output: 3
   ```

In both cases, the destructuring syntax allows you to conveniently extract values from objects or arrays and assign them to variables with a concise syntax. It helps avoid repeated references to object properties or array indices and makes the code more readable and expressive.

# Q.9 How can you define default parameter values in ES6 functions?

Ans: To define default parameter values in ES6 functions, you can assign a default value directly to the function parameter using the `=` operator. If the parameter is not provided or is `undefined`, the default value will be used. It allows you to handle missing or undefined function arguments easily.

# Q.10 What is the purpose of the spread operator (...) in ES6?

Ans: The spread operator (`...`) in ES6 allows you to expand elements from an iterable (like an array or string) into individual elements. It is useful for tasks such as creating new arrays, copying arrays, merging objects, passing multiple function arguments, and manipulating strings. The spread operator provides a concise and versatile way to work with data in different contexts.