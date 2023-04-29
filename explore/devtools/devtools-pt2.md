# Part 1

## Question 1

1. What was the bug?

**The funciton was concatinating them as strings and returning a string instead of adding the two numbers together.**

## Question 2

2. How would you fix it? Include a screenshot of your fix. Name it fix.png (or whatever image extension you would like to use)

**I would parse num1 and num2 as ints like:**
`let result = parseInt(num1) + parseInt(num2);`