**1.** `3` is printed. `i` is defined as 0 and increments 3 times because the length of `prices` is 3. Since `i` is defined using `var`, its scope is the entire function `discountPrices`, so it is still defined on line 12. Thus, after the `for` loop, `i` is 3.

**2.** `150` is printed. The last time `discountedPrice` is defined is when `prices[i]` is 300, so it will be set to 150 when the `for` loop ends. Since it is defined using `var`, it will still be defined on line 13.

**3.** `150` is printed. The last time `finalPrice` is updated is when `discountedPrice` is 150, so the rounding will not change the value. Since `finalPrice` is defined using `var`, it will still be defined on line 14.

**4.** The function will return `[50, 100, 150]`. It applies the discount to each value in the inputted array and returns a new array containing the updated prices. In this case, it applies a 50% discount to 100, 200, and 300.

**5.** The code causes an error because `i` is defined using `let`, so its scope is only within the `for` loop. On line 12, `i` is undefined.

**6.** The code causes an error because similarly to Question 5, `discountedPrice` is defined using `let`, so its scope is only within the `for` loop. On line 13, `discountedPrice` is undefined.

**7.** Line 14 prints `150`. Even though `finalPrice` is defined using `let`, it is defined outside of the `for` loop, so its scope is the whole function. For the same reason as in Question 3, `finalPrice`'s value will be 150.

**8.** The function will return `[50, 100, 150]` just like in Question 4. `discounted`'s scope is the entire function, so it is still defined on line 16, and thus the returned array is still correct.

**9.** The code causes an error for the same reason as in Question 5. `i` is out of scope on line 11.

**10.** Line 12 prints `3`. `length`'s scope is the entire function, and its value is 3 throughout the function.

**11.** The function will return `[50, 100, 150]`, just like in Question 4. Although `discounted` is now defined using `const`, it can still be changed as long as it is not reassigned, so the result is unchanged.

**12A.** `student.name` \
**12B.** `student['Grad Year']` \
**12C.** `student.greeting()` \
**12D.** `student['Favorite Teacher'].name` \
**12E.** `student.courseLoad[0]`

**13A.** `'32'`. `2` gets converted into a string. \
**13B.** `1`. `'3'` gets converted into a number. \
**13C.** `3`. `null` gets converted into the number `0`. \
**13D.** `'3null'`. `null` becomes a string. \
**13E.** `4`. `true` becomes the number `1`. \
**13F.** `0`. `false` and `null` both become the number `0`. \
**13G.** `'3undefined'`. `undefined` becomes a string. \
**13H.** `NaN`. `'3'` becomes a number and JavaScript tries to convert `undefined` into a number, which causes it to become `NaN`.

**14A.** `true`. `'2'` becomes a number. \
**14B.** `false`. Alphabetically, the string `'1'` is less than the string `'2'`. \
**14C.** `true`. The string `'2'` becomes a number due to the double equality sign `==`. \
**14D.** `false`. The triple equality sign `===` does not perform type conversion. \
**14E.** `false`. `true` becomes the number `1`. \
**14F.** `true`. The explicit `Boolean()` conversion becomes `true` for any intuitively "non-empty" input, so `Boolean(2)` becomes `true`.

**15.** `==` performs type conversion before the comparison, while `===` does not.

**17.** `[2, 4, 6]` is the array returned by line 13. The `modifyArray` function takes an array and a callback function as input. It calls the callback function on each item in the array, and outputs an array containing each result. The `doSomething` function that is given to `modifyArray` as the callback function multiplies its input by 2, so line 13 multiplies each item in the array by 2.

**19.** The output is `1`, `4`, `3`, and `2` on separate lines in that order.