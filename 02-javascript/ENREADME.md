# Javascript

"Javascript is not Java, not even related."

## Contents to be covered

## Control structures

Control structures are used to control the flow of execution of a program. JavaScript has several control structures, including `if` statements, `for` loops, `while` loops, `switch` statements, and `try/catch` blocks. These structures allow you to execute different blocks of code depending on certain conditions or to repeat a block of code multiple times.

## Differences between `var`, `let`, `const`

In JavaScript, `var`, `let`, and `const` are used to declare variables. `var` is the old way of declaring variables, while `let` and `const` are newer and were introduced in ES6. The main differences between them are that `var` has function scope, while `let` and `const` have block scope, and that `const` cannot be reassigned after it's been initialized.

For example:

```// Using var
function exampleVar() {
  var x = 10;
  if (true) {
    var x = 20; // This reassigns the same variable declared above
    console.log(x); // Output: 20
  }
  console.log(x); // Output: 20 (the same value as the previous console.log)
}

// Using let
function exampleLet() {
  let x = 10;
  if (true) {
    let x = 20; // This declares a new variable with the same name but with block scope
    console.log(x); // Output: 20
  }
  console.log(x); // Output: 10 (the value of the variable declared above)
}

// Using const
function exampleConst() {
  const x = 10;
  if (true) {
    // const x = 20; // This would cause an error since you cannot reassign a constant variable
    console.log(x); // Output: 10
  }
  console.log(x); // Output: 10 (the same value as the previous console.log)
}
```

In the `exampleVar()` function, the `var` keyword is used to declare a variable `x` with function scope. The if block inside the function reassigns the same variable `x` to a new value of 20, and that change is reflected in the second `console.log()` statement outside the block.

In the `exampleLet()` function, the let keyword is used to declare a variable `x` with block scope. The if block inside the function declares a new variable `x` with the same name and reassigns it to a value of 20. However, that change does not affect the value of the `x` variable declared outside the block, so the first `console.log()` statement inside the block outputs 20 while the second `console.log()` statement outside the block outputs 10.

In the `exampleConst()` function, the const keyword is used to declare a constant variable `x` with block scope. Since constants cannot be reassigned after they've been initialized, attempting to reassign `x` inside the if block would cause an error. The first and second `console.log()` statements output the same value of 10 since `x` has not been changed.



## Named and anonymous functions
## Object destructuring & spreading
## Array destructuring & spreading
## Promises and async/await
## Comparisons in Javascript
## == vs. === - Differences to Java
## Truthy and falsy
## Array functions map, filter, find, reduce, forEach, some, every
## Further links"