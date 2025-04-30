# Part 1: JavaScript Variable Declarations

## Question 1
**What is printed by line 9?**  
Output: `values added: 20`  
Because `var` is function scoped, and `result = num1 + num2` is executed correctly.

## Question 2
**What is printed by line 13?**  
Output: `final result: 20`  
`var result` is accessible even outside the `if` block due to function scope.

## Question 3
**Why should you not use var?**  
Because `var` is function-scoped, not block-scoped. This can lead to accidental reuse of variable names and bugs due to unexpected access outside a block. `let` and `const` are block-scoped and safer to use.

---

## Question 4
**What is printed by line 9?**  
Output: `values added: 20`  
`let result` is scoped inside the `if` block and works fine within it.

## Question 5
**What is printed by line 13?**  
Error: `ReferenceError: result is not defined`  
Because `let` is block-scoped, and line 13 is outside the `if` block.

---

## Question 6
**What is printed by line 9?**  
Error: `TypeError: Assignment to constant variable.`  
cannot reassign a `const` variable after it's initialized.

## Question 7
**What is printed by line 13?**  
Line 9 already throws an error, so this line will never execute.
