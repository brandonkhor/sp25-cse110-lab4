1. Line 12 will print `3` in the console because on line 6, we declare `i` as a `var`, meaning its scope isn't limited to the `for` block and can be used outside of it. In the given example, `prices` has a length of 3, so the `for` loop will break once `i` reaches 3.
2. Line 13 will print `150` in the console. Since `discountedPrice` is a `var`, it can be used outside the block it was defined in. We can see that for each iteration of the for loop, `var discountedPrice = prices[i] * (1 - discount)`, so the value of `discountedPrice` will be for the last element of `prices`, which is `300`. If we plug it in with `discount = 0.5`, we get 300 * (1-0.5) = 150.
3. Line 14 will print `150` in the console. Since `finalPrice` is a `var`, it has a function scope. We set `finalPrice = Math.round(discountedPrice * 100) / 100`. As seen in 2, the last value of `discountedPrice` will be `150`. Plugging this into `finalPrice`, we get `150`.
4. The function will return an array containing each element in `prices` after the discount and rounding is applied. The final result of `discounted` is `[ 50, 100, 150 ]`
5. This will cause an error. On line 6, we declare `i` as a `let`, making it block-scoped. Since the `for` block is lines 6-10 and line 12 is outside this block, we can no longer access `i` from this line, throwing an error.
6. This will cause an error. On line 7, we declare `discountedPrice` as a `let`, making it block-scoped. Since the `for` block is lines 6-10 and line 13 is outside this block, we can no longer access `discountedPrice` from this line, throwing an error.
7. Line 14 will print `150` in the console. Even though `finalPrice` is a `let` and it has a block scope, it is declared on line 4, which is not in any block (technically in the function's block). We set `finalPrice = Math.round(discountedPrice * 100) / 100`. As seen in 2, the last value of `discountedPrice` will be `150`. Plugging this into `finalPrice`, we get `150`.
8. The function will return an array containing each element in `prices` after the discount and rounding is applied. The final result of `discounted` is `[ 50, 100, 150 ]`. Even though `discounted` is now a `let`, aswell as related variables like `finalPrice`, `i`, and `discountedPrice`, none of the related variables are called outside their respective block and `discounted` is declared outside any specific block, allowing us to use it anywhere in the function.
9. This will cause an error. On line 6, we declare `i` as a `let`, making it block-scoped. Since the `for` block is lines 6-9 and line 11 is outside this block, we can no longer access `i` from this line, throwing an error.
10. Line 12 will print `3` in the console because on line 4, we declare `length` as a `const`, meaning it's block-scoped and the value cannot be changed. However, line 4 isn't contained in any block, so it can be used throughout the function. `Length` is never changed in anyway, so no error there. Since `prices` contains 3 elements, `length` is 3.
11. The function will return `discounted` which is `[ 50, 100, 150 ]`. In the `for` loop, we are declaring and pushing `discountedPrice`. Even though it is a `const`, we are never changing its value after it is declared. Rather, we are just redeclaring it for each iteration of the loop, allowing us to "change" the value of `discountedPrice` for each iteration.
12. <br> A. student.name
    <br> B. student["Grad Year"]
    <br> C. student.greeting()
    <br> D. student["Favorite Teacher"].name
    <br> E. student.coarseLoad[0]
13. <br> A. '3' + 2 = '32' since integers map to their exact string representation
    <br> B. '3' - 2 = 1 due to the -, '3' becomes the integer 3, making it simple arithmetic
    <br> C. 3 + null = 3 because null is converted to a 0, so 3 + 0 = 3
    <br> D. '3' + null = '3null' because null is converted to a string due to string concatenation
    <br> E. true + 3 = 4 because true turns into 1, so 1 + 3 = 4
    <br> F. false + null = 0 because as mentioned in C, null is 0, and false turns into 0
    <br> G. '3' + undefined = '3underfined' because like D, the underfined is converted to a string due to string concatenation
    <br> H. '3' - undefined = NaN because like B, '3' becomes the integer 3, and subtracting undefined makes it NaN
14. <br> A. '2' > 1 **true**, '2' is convert to the integer 2, so 2 > 1 = true
    <br> B. '2' < '12' **false**, since they're both strings, it is compared lexicographically, and since '2' comes after '1', it is false
    <br> C. 2 == '2' **true**, == allows for type coercion, so '2' becomes 2
    <br> D. 2 === '2' **false**, === requires the types and values to be the same, so results to false
    <br> E. true == 2 **false**, true becomes 1, and since 1 != 2, we get false
    <br> F. true === Boolean(2) **true**, Boolean(0) is the only thing that evaluates to false, so Boolean(2) is true, so true
15. == compares the values (can do type coercion), whereas === compares the types and the values (no type coercion)
16. See js file
17. The result will be `[2,4,6]`. It iterates through the array `[1,2,3]` and applies the callback function to each element, which doubles the element. Each of these new doubled elements are pushed to `newArr`, which is then returned, giving us our result.
18. See js file
19. 1
<br> 4
<br> 3
<br> 2
