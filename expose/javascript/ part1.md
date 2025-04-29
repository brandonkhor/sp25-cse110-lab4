1. values added:  20
2. final result:  20
3. Can lead to naming conflicts and scoping issues. Since `var` is function-scoped (compared to block-scoped like `const` and `let`), issues can arise if it is used inside a block (Ex. Using same `var` name outside AND inside a block).

4. values added:  20
5. Error, says that `result` isn't defined because `let` is block-scoped, meaning that once we exit the block, we cannot access it anymore. This can be seen on line 13, which is outside the lines 3-11 block.

6. Error, `const result` is set to 0 on line 5, meaning that this value is final and cannot be changed. When we try to change it on line 7, an error is thrown.
7. Error, says that `result` isn't defined because `const` is block-scoped, meaning that once we exit the block, we cannot access it anymore. This can be seen on line 13, which is outside the lines 3-11 block.
