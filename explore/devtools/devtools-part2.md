1. The bug is that `num1` and `num2` are strings, which can be seen when result is of type string. This causes string concatenation instead of addition arithmetic
2. Parse `num1` and `num2` as numbers using `Number()`, allowing for addition rather than string concatenation.
