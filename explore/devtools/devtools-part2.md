## DevTools - Debugging

### 1. What was the bug?
The bug was that the two input values `num1` and `num2` were being treated as strings rather than numbers. When using the `+` operator with strings, it performs concatenation instead of arithmetic addition. As a result, entering 11 and 22 gave "1122" instead of 33.

### 2. How would you fix it?
To fix this, I would convert the inputs to numbers before adding them. This can be done using `Number()` or `parseInt()`:

```js
function calculateSum(num1, num2) {
  let result = Number(num1) + Number(num2);
  return result;
}
