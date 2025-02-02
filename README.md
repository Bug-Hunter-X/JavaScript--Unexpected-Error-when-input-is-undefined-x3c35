# JavaScript Unexpected Error when Input is Undefined

This repository demonstrates a common JavaScript error related to handling undefined values. The `foo` function attempts to access the `length` property of the input `x`. However, it fails to handle the case where `x` is undefined, resulting in an error.

## Bug

The provided `bug.js` file contains a function that incorrectly handles undefined input. When an undefined value is passed to the function, it will throw a TypeError because it attempts to access the `length` property of `undefined`.

## Solution

The `bugSolution.js` file provides a corrected version of the function.  It explicitly checks for both `null` and `undefined` before attempting to access the `length` property, preventing the error.

## How to reproduce

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js`
3. Run the code in a JavaScript environment (browser's console, Node.js, etc.).
4. Call the `foo` function with an undefined value in `bug.js`. Observe the error.
5. Call the `foo` function with an undefined value in `bugSolution.js`. Observe the corrected behaviour. 