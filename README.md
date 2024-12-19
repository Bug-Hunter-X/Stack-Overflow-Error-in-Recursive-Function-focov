# Stack Overflow Bug in JavaScript

This repository demonstrates a common error in JavaScript: stack overflow errors caused by unbounded recursion.

## The Bug

The `bug.js` file contains a recursive function `foo()`.  This function works correctly for small inputs but will crash the program for larger inputs, due to exceeding the maximum call stack size.

## The Solution

The `bugSolution.js` file provides a corrected version of the function, adding a check to prevent unbounded recursion. This improved version uses iteration rather than recursion to avoid the stack overflow problem. 

## How to Reproduce

1. Clone this repository.
2. Run `bug.js` with a large value as input for `a`.  Observe the error.
3. Run `bugSolution.js` with the same input value. Observe the correct output.

This example illustrates the importance of carefully considering recursion depth and implementing appropriate safeguards to prevent stack overflow errors.