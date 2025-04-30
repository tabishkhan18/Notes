# JavaScript Interview Questions and Answers

# JavaScript

<!----------------------------------------------------------------------------------------------------------->

    (Q.1)=> Define JavaScript?

    - JavaScript is a single-threaded, syncronous, high-level interpreted programming language. 
      which is used to create interactive and dynamic content on websites. It is one of the core technologies that is used in web development as a scipting language, alongside with HTML and CSS. 

<!----------------------------------------------------------------------------------------------------------->

    (Q.2)=> Variables in JavaScript

    - There are 3 types of variables available in JavaScipt, var, let and const. var is function level scoped
      while let and const are block level scoped. Value of let and var can be reassigned whereas the value of const cannot. In modern javascript, most of the programmers prefer to avoid using var because of it lacks block level scoping and due to hoisting.

<!----------------------------------------------------------------------------------------------------------->

    (Q.3)=> Datatypes in JavaScript

    - Datatypes in JavaScript are divided in two categories:-
      1 - 7 Primitive: (Number, String, Boolean, Null, Undefined, BigInt, Symbol)
          // Stored by value
      2 - 3 Non-Primitive/Reference: (Array, Object, Function) 
          // Stored by reference

    Note: Primitive datatypes are immutable, meaning they cannot be changed once created. Non-primitive datatypes are mutable, meaning they can be changed after creation.
    Note: Primitive datatypes are stored in the stack memory, while non-primitive datatypes are stored in the heap memory.

<!----------------------------------------------------------------------------------------------------------->


    (Q.4)=> Type Conversion and Coercion

    - Type conversion an explicit conversion process of variable's datatype(ex: Number("123) ), while coercion is an automatic behaviour of JavaScript that convert variable's datatype (ex: "5" + 5 = "55"). To avoid unexpected coercion, use "===".

    - Type conversion is the process of converting one data type to another. JavaScript provides several methods for type conversion, including:
      1 - Number(): Converts a value to a number.
      2 - String(): Converts a value to a string.
      3 - Boolean(): Converts a value to a boolean.
      4 - parseInt(): Converts a string to an integer.
      5 - parseFloat(): Converts a string to a floating-point number.

<!----------------------------------------------------------------------------------------------------------->

    (Q.5)=> Operators in JavaScript

    - Types of operators in JavaScript:
        1 - Arithematic ( +, -, *, /, % )
        2 - Comparision ( >, <, >=, <=, ==, ===, !=, !== )
        3 - Logical ( &&, ||, ! )
        4 - Assignment ( =, += )

    Note: "==" check the value, "===" check the value and type also. Prefer "===".


<!----------------------------------------------------------------------------------------------------------->

    (Q.6)=> Conditional Statements in JavaScript

    - Conditional statements are used to perform different actions based on different conditions. 
      1 - if
      2 - else if
      3 - else
      4 - switch: switch is used when there are multiple possible values for a variable.

    Note: Ternary (condition ? a : b) is a shorthand for simple conditions. 


<!----------------------------------------------------------------------------------------------------------->

    (Q.7)=> Loops in JavaScript

    - Loops are used to execute a block of code repeatedly until a specified condition is met.
      1 - for: for loop is used to execute a block of code a specified number of times.
      2 - while: while loop is used to execute a block of code as long as a specified condition is true.
      3 - do while: do while loop is similar to while loop, but it executes the block of code at least once before checking the condition.
      4 - for in: for in is used to iterate over the properties of an object.
      5 - for of: for of is used to iterate over iterable objects like arrays and strings.
      6 - forEach: forEach is a method of arrays that executes a provided function once for each array element. It does not return a new array and cannot be used with break or continue statements.

<!----------------------------------------------------------------------------------------------------------->

    (Q.8)=> Functions in JavaScript

    - Functions are reusable blocks of code that perform a specific task. 
      1 - Function Expression: Function Expression is a function that is assigned to a variable
      2 - Function Declaration: Function Declaration is a function that is defined with the "function" keyword.
      3 - Arrow Function: Arrow functions do not have their own "this" context, suitable for callbacks.
      4 - IIFE (Immediately Invoked Function Expression): IIFE is a function that runs as soon as it is defined. It is used to create a new scope and avoid polluting the global scope.

    Note: Function Declaration is hoisted, while Function Expression and Arrow Function are not hoisted.


<!----------------------------------------------------------------------------------------------------------->

    (Q.9)=> Scope in JavaScript

    - Scope refers to the visibility of variables and functions in a particular context. 
      1 - Global Scope
      2 - Local Scope
      3 - Block Scope
      4 - Lexical Scope

    Note: Global scope is accessible from anywhere in the code, while local scope is only accessible within the function or block it is defined in.
    Note: Block scope is created by using let and const keywords, while lexical scope is created by using function declarations.


<!----------------------------------------------------------------------------------------------------------->

    (Q.10)=> Hoisting in JavaScript

    - Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope during the compile phase. 
      1 - Variable Hoisting: Variables declared with var are hoisted to the top of their scope, but their values are not assigned until the line of code is executed.
      2 - Function Hoisting: Function declarations are hoisted to the top of their scope, allowing them to be called before they are defined in the code.

    Note: Hoisting does not apply to let and const variables, as they are block-scoped and cannot be accessed before their declaration.

<!----------------------------------------------------------------------------------------------------------->

    (Q.11)=> Closures in JavaScript

    - A closure is a function that has access to its outer function's scope, even after the outer function has returned. 
      1 - Closure Example: A closure can be used to create private variables and functions.

    Note: Closures are useful for data encapsulation and creating private variables.
    Note: Closures can lead to memory leaks if not handled properly, as they can keep references to variables that are no longer needed.

<!----------------------------------------------------------------------------------------------------------->

    (Q.12)=> Callbacks in JavaScript

    - A callback is a function that is passed as an argument to another function and is executed after the completion of that function. 
      1 - Callback Example: Callbacks are commonly used in asynchronous programming, such as with event listeners and AJAX requests.

    Note: Callbacks can lead to "callback hell" if not managed properly, making the code difficult to read and maintain.
    Note: Promises and async/await are modern alternatives to callbacks for handling asynchronous operations.

<!----------------------------------------------------------------------------------------------------------->

    (Q.13)=> Promises in JavaScript

    - A promise is an object that represents the eventual completion (or failure) of an asynchronous operation and its resulting value. 
      1 - Promise States: A promise can be in one of three states: pending, fulfilled, or rejected.
      2 - Promise Example: Promises are commonly used for handling asynchronous operations, such as API calls.

    Note: Promises can be chained using the .then() method to handle multiple asynchronous operations in a more readable way.
    Note: The .catch() method is used to handle errors in promises.

<!----------------------------------------------------------------------------------------------------------->

    (Q.14)=> Async/Await in JavaScript

    - Async/await is a modern way to handle asynchronous operations in JavaScript, making the code more readable and easier to understand. 
      1 - Async Function: An async function is a function that returns a promise and allows the use of the await keyword inside it.
      2 - Await Keyword: The await keyword is used to pause the execution of an async function until the promise is resolved.

    Note: Async/await is built on top of promises and provides a cleaner syntax for handling asynchronous operations.
    Note: Error handling in async/await can be done using try/catch blocks.

<!----------------------------------------------------------------------------------------------------------->

    (Q.15)=> Event Loop in JavaScript

    - The event loop is a mechanism that allows JavaScript to perform non-blocking I/O operations, even though JavaScript is single-threaded. 
      1 - Call Stack: The call stack is a data structure that keeps track of function calls in the order they are made.
      2 - Callback Queue: The callback queue is a queue that holds messages and their associated callback functions.
      3 - Event Loop: The event loop continuously checks the call stack and the callback queue, executing the callback functions when the call stack is empty.

    Note: The event loop allows JavaScript to handle asynchronous operations without blocking the main thread.
    Note: Understanding the event loop is crucial for writing efficient and responsive JavaScript applications.

<!----------------------------------------------------------------------------------------------------------->

    (Q.16)=> DOM Manipulation in JavaScript

    - The Document Object Model (DOM) is a programming interface for web documents, representing the structure of a document as a tree of objects. 
      1 - Selecting Elements: JavaScript provides several methods for selecting elements in the DOM, such as getElementById(), querySelector(), and getElementsByClassName().
      2 - Modifying Elements: JavaScript can be used to modify the content, attributes, and styles of DOM elements using properties like innerHTML, setAttribute(), and style.
      3 - Event Handling: JavaScript can be used to add event listeners to DOM elements, allowing for interactive web pages.

    Note: DOM manipulation is a powerful feature of JavaScript that allows developers to create dynamic and interactive web applications.
    Note: Excessive DOM manipulation can lead to performance issues, so it's important to optimize the code for better performance.

<!----------------------------------------------------------------------------------------------------------->

    (Q.17)=> ES6 Features in JavaScript

    - ES6 (ECMAScript 2015) introduced several new features and improvements to JavaScript, including:
      1 - let and const: Block-scoped variables and constants.
      2 - Arrow Functions: Shorter syntax for writing functions.
      3 - Template Literals: String interpolation and multi-line strings using backticks.
      4 - Destructuring Assignment: Extracting values from arrays or objects into variables.
      5 - Spread and Rest Operators: Expanding or collecting elements in arrays or function arguments.
      6 - Promises: A new way to handle asynchronous operations.
      7 - Modules: Support for modular programming with import/export syntax.

    Note: ES6 features are widely supported in modern browsers, making it easier to write cleaner and more efficient code.
    Note: Understanding ES6 features is essential for modern JavaScript development and working with frameworks like React and Vue.js.

<!----------------------------------------------------------------------------------------------------------->

    (Q.18)=> Object-Oriented Programming in JavaScript

    - Object-oriented programming (OOP) is a programming paradigm that uses objects to represent data and methods. 
      1 - Objects: Objects are collections of key-value pairs, where keys are strings and values can be any data type.
      2 - Classes: Classes are blueprints for creating objects, allowing for inheritance and encapsulation.
      3 - Prototypes: Prototypes are the mechanism by which JavaScript objects inherit properties and methods from other objects.

    Note: OOP allows for better organization of code and promotes reusability and maintainability.
    Note: Understanding OOP concepts is important for working with JavaScript frameworks and libraries.

<!----------------------------------------------------------------------------------------------------------->

    (Q.19)=> Functional Programming in JavaScript

    - Functional programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing state or mutable data. 
      1 - First-Class Functions: Functions are treated as first-class citizens, meaning they can be passed as arguments, returned from other functions, and assigned to variables.
      2 - Higher-Order Functions: Functions that take other functions as arguments or return functions as their result.
      3 - Pure Functions: Functions that always produce the same output for the same input and have no side effects.

    Note: Functional programming promotes immutability and statelessness, making it easier to reason about code and avoid bugs.
    Note: Understanding functional programming concepts is beneficial for writing clean and maintainable JavaScript code.

<!----------------------------------------------------------------------------------------------------------->

    (Q.20)=> Error Handling in JavaScript

    - Error handling is the process of responding to and recovering from error conditions in a program. 
      1 - try/catch: The try/catch statement is used to handle exceptions in JavaScript.
      2 - throw: The throw statement is used to create custom errors.
      3 - finally: The finally block is executed after the try/catch block, regardless of whether an error occurred.

    Note: Proper error handling is important for creating robust and user-friendly applications.
    Note: Using try/catch blocks can help prevent crashes and provide meaningful error messages to users.

<!----------------------------------------------------------------------------------------------------------->

    (Q.21)=> JSON in JavaScript

    - JSON (JavaScript Object Notation) is a lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate. 
      1 - JSON Syntax: JSON data is represented as key-value pairs, similar to JavaScript objects.
      2 - JSON Methods: JavaScript provides two methods for working with JSON: JSON.stringify() for converting JavaScript objects to JSON strings and JSON.parse() for converting JSON strings to JavaScript objects.

    Note: JSON is commonly used for data exchange between a server and a client in web applications.
    Note: Understanding JSON is essential for working with APIs and handling data in JavaScript applications.

<!----------------------------------------------------------------------------------------------------------->

    (Q.22)=> Local Storage and Session Storage in JavaScript

    - Local storage and session storage are web storage APIs that allow developers to store data in the browser. 
      1 - Local Storage: Local storage is used to store data with no expiration time, meaning the data persists even after the browser is closed.
      2 - Session Storage: Session storage is used to store data for the duration of the page session, meaning the data is cleared when the page session ends.

    Note: Both local storage and session storage store data as key-value pairs and have a maximum storage limit of around 5-10MB.
    Note: Web storage APIs are useful for storing user preferences, authentication tokens, and other data that needs to persist across page reloads or sessions.

<!----------------------------------------------------------------------------------------------------------->

    
