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
