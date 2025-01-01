# Unhandled Non-Number Input in TypeScript Arithmetic Functions

This repository demonstrates a common, yet subtle, bug in TypeScript:  failure to handle non-number inputs in arithmetic functions.

The `bug.ts` file contains the original code with the bug. The `bugSolution.ts` file provides a solution that includes input validation.

## Bug

The `divide` function correctly handles division by zero. However, it doesn't check if the inputs (`a` and `b`) are actually numbers.  If non-numeric values are passed, unexpected behavior or runtime errors will occur.

## Solution

The solution involves adding input validation to ensure both `a` and `b` are numbers before performing the arithmetic operations.  Type guards or explicit type checks can be used to achieve this.