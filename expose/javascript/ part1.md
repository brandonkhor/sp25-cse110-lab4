1. values added:  20
2. final result:  20
3. Can lead to naming conflicts and scoping issues. Since `var` is function-scoped (compared to block-scoped like `const` and `let`), issues can arise if it is used inside a block (Ex. Using same `var` name outside AND inside a block).

4. values added:  20
5. Error, says that result isn't defined because `let` is block-scoped, meaning that once we exit the block, we cannot access it anymore. This can be seen on line 13, which is outside the 3-11 block.
