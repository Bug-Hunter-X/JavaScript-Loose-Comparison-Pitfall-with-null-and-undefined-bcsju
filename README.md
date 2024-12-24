# JavaScript Loose Comparison Pitfall with null and undefined

This repository demonstrates a common JavaScript error related to loose comparison (==) of null and undefined values.  The `foo` function attempts to handle null values gracefully, but it fails to explicitly handle undefined, resulting in unexpected NaN (Not a Number) output.

## Bug

The `bug.js` file shows the problematic code.  The loose comparison `x === null` only checks for null and not undefined, leading to NaN when undefined is passed.  Strict equality (`===`) should be used for accurate comparisons.

## Solution

The `bugSolution.js` file provides a corrected version. It explicitly checks for both null and undefined using strict equality (`===`), ensuring proper handling of both cases.
