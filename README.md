# JavaScript Bug: Handling Undefined in Length Check

This repository demonstrates a common JavaScript error: attempting to access the `length` property of an undefined value.  The original code throws a `TypeError`.  The solution provides a robust way to handle undefined values gracefully.

## Bug

The `foo` function attempts to determine the length of the input `x`.  It handles `null` correctly, but fails when called with `undefined`. 

## Solution

The solution adds a check for `undefined` before accessing `x.length`. This prevents the `TypeError` and returns a meaningful value instead.