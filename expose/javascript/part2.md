**Question 1:** `3` is printed. `i` is defined as 0 and increments 3 times because the length of `prices` is 3. Since `i` is defined using `var`, its scope is the entire function `discountPrices`, so it is still defined on line 12. Thus, after the `for` loop, `i` is 3.

**Question 2:** `150` is printed. The last time `discountedPrice` is defined is when `prices[i]` is 300, so it will be set to 150 when the `for` loop ends. Since it is defined using `var`, it will still be defined on line 13.

**Question 3:** `150` is printed. The last time `finalPrice` is updated is when `discountedPrice` is 150, so the rounding will not change the value. Since `finalPrice` is defined using `var`, it will still be defined on line 14.

**Question 4:** The function will return `[50, 100, 150]`. It applies the discount to each value in the inputted array and returns a new array containing the updated prices. In this case, it applies a 50% discount to 100, 200, and 300.

**Question 5:** The code causes an error because `i` is defined using `let`, so its scope is only within the `for` loop. On line 12, `i` is undefined.

**Question 6:** The code causes an error because similarly to Question 5, `discountedPrice` is defined using `let`, so its scope is only within the `for` loop. On line 13, `discountedPrice` is undefined.

**Question 7:** Line 14 prints `150`. Even though `finalPrice` is defined using `let`, it is defined outside of the `for` loop, so its scope is the whole function. For the same reason as in Question 3, `finalPrice`'s value will be 150.

**Question 8:** The function will return `[50, 100, 150]` just like in Question 4. `discounted`'s scope is the entire function, so it is still defined on line 16, and thus the returned array is still correct.

**Question 9:** The code causes an error for the same reason as in Question 5. `i` is out of scope on line 11.

**Question 10:** Line 12 prints `3`. `length`'s scope is the entire function, and its value is 3 throughout the function.

**Question 11:** The function will return `[50, 100, 150]`, just like in Question 4. Although `discounted` is now defined using `const`, it can still be changed as long as it is not reassigned, so the result is unchanged.