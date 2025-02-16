# JavaScript Loose Comparison Bug

This repository demonstrates a common JavaScript bug involving loose comparison (==) with null and undefined values in an addition function.

The `foo` function is designed to add two numbers, but it handles null values correctly. However, it does not handle undefined values gracefully, resulting in NaN (Not a Number). This highlights a subtle difference in how JavaScript treats null and undefined in loose comparisons.

## Bug
The `bug.js` file contains the buggy code.  Observe the output in the console.  The unexpected NaN output when using undefined illustrates the core issue.

## Solution
The `bugSolution.js` file provides a corrected version of the function, using strict equality (===) for more precise comparison and handling undefined and null more robustly.  This improves the function's reliability and predictability.  