**1.** The bug was that `num1` and `num2` were being interpreted as strings, so `result` was actually a string variable containing the concatenation of the strings `num1` and `num2`, instead of their sum.

**2.** I would fix the bug by changing explicitly converting `num1` and `num2` to numbers. \
Before: `let result = num1 + num2` \
After: `let result = Number(num1) + Number(num2)`