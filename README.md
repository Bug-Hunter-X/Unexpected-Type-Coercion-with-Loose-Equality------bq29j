# Unexpected Type Coercion with Loose Equality (==) in JavaScript

This repository demonstrates a common JavaScript bug related to loose equality (==) and null/undefined values.  Loose equality can lead to unexpected type coercion, resulting in incorrect comparisons and potentially hard-to-debug errors.

## The Bug

The `bug.js` file contains a function that uses loose equality.  The problem arises when the function receives `null` or `undefined` as arguments.  Loose equality performs type coercion before comparison, leading to incorrect results.

## The Solution

The `bugSolution.js` file presents a corrected version using strict equality (===).  Strict equality does not perform type coercion, providing a more reliable and predictable comparison.

## How to reproduce the bug

1. Clone this repository.
2. Run `node bug.js` and observe the output.
3. Run `node bugSolution.js` and observe the corrected output.