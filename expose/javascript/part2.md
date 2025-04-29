# Part 2 - JavaScript Scope and Behavior

## Question 1  
Output: 3  
Explanation: `var i` is function scoped, so it is still accessible outside the for loop.

## Question 2  
Output: 150  
Explanation: `var discountedPrice` is also function scoped. Last value remains accessible.

## Question 3  
Output: 150  
Explanation: `finalPrice` was last set to 150. `var` allows access anywhere in the function.

## Question 4  
Output: `[50, 100, 150]`  
Explanation: Each value is halved and rounded correctly into the array.

## Question 5  
Error: `i is not defined`  
Explanation: `let i` is block scoped, not visible outside the loop.

## Question 6  
Error: `discountedPrice is not defined`  
Explanation: Same, `let discountedPrice` is block scoped inside the loop.

## Question 7  
Output: 150  
Explanation: `finalPrice` was declared with `let` in the outer scope, accessible.

## Question 8  
Output: `[50, 100, 150]`  
Explanation: Code logic is correct, using block-scoped variables properly.

## Question 9  
Error: `i is not defined`  
Explanation: `let i` was declared inside loop, not accessible at line 11.

## Question 10  
Output: 3  
Explanation: `const length` was declared in function scope, accessible at line 12.

## Question 11  
Output: `[50, 100, 150]`  
Explanation: Prices are correctly halved and pushed into the array.

## Question 12: Object Property Access
```js
A. student.name
B. student["Grad Year"]
C. student.greeting()
D. student["Favorite Teacher"].name
E. student.courseLoad[0]
```

## Question 13: Type Conversion Outputs
```js
A. '3' + 2 → '32'      // String + number = string concatenation
B. '3' - 2 → 1         // String - number = coerced to number
C. 3 + null → 3        // null is coerced to 0
D. '3' + null → '3null' // String + null = string
E. true + 3 → 4        // true = 1
F. false + null → 0    // false = 0, null = 0
G. '3' + undefined → '3undefined' // string + undefined
H. '3' - undefined → NaN // undefined becomes NaN in math
```

## Question 14: Comparison Outputs
```js
A. '2' > 1 → true      // '2' becomes number
B. '2' < '12' → false  // lexicographic string comparison
C. 2 == '2' → true     // loose equality with type coercion
D. 2 === '2' → false   // strict equality, type mismatch
E. true == 2 → false   // true = 1, 1 != 2
F. true === Boolean(2) → true // Boolean(2) is true
```

## Question 15: Difference between `==` and `===`

`==` does **type coercion**, meaning it converts values to the same type before comparing.  
`===` checks both **value and type** — no type conversion.

## Question 16: for...in loop (part2-question16.js)
Print properties of `statistics` if:
- Key starts with `'r'`
- Or value is an odd number

```js
for (let key in statistics) {
  if (key[0] === 'r' || statistics[key] % 2 === 1) {
    console.log(statistics[key]);
  }
}
