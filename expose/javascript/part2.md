**Question 1:** `3` is printed. `i` is defined as 0 and increments 3 times because the length of `prices` is 3. Since `i` is defined using `var`, its scope is the entire function `discountPrices`, so it is still defined on line 12. Thus, after the `for` loop, `i` is 3.

**Question 2:** `150` is printed. The last time `discountedPrice` is defined is when `prices[i]` is 300, so it will be set to 150 when the `for` loop ends. Since it is defined using `var`, it will still be defined on line 13.

**Question 3:** `150` is printed. The last time `finalPrice` is updated is when `discountedPrice` is 150, so the rounding will not change the value. Since `finalPrice` is defined using `var`, it will still be defined on line 14.

**Question 4:** The function will return `[50, 100, 150]`. It applies the discount to each value in the inputted array and returns a new array containing the updated prices. In this case, it applies a 50% discount to 100, 200, and 300.

**Question 5:**