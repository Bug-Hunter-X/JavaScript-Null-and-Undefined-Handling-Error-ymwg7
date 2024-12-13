# JavaScript Null and Undefined Handling

This repository demonstrates a common error in JavaScript involving the handling of `null` and `undefined` values.  The initial code snippet handles `null` correctly but fails to explicitly check for `undefined`.  The corrected solution addresses this by including checks for both `null` and `undefined`.

## Bug
The `foo` function correctly returns `null` if either input is `null`. However, if either `a` or `b` is `undefined`, unexpected behavior (NaN) can result. This is because `undefined` + number is NaN. The solution provides a more robust handling for null and undefined inputs.

## Solution
The solution enhances the function to explicitly check for both `null` and `undefined`, resulting in more predictable and reliable behavior.  The modified function returns `0` if either input is undefined or null to provide default behaviour.  A better solution might be to throw an error instead. 