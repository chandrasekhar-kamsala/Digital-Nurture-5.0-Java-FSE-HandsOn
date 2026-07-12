# Exercise 7: Financial Forecasting

## Scenario

You are developing a financial forecasting tool that predicts future values based on past data.

---

## Objective

- Understand recursion.
- Implement a recursive algorithm for financial forecasting.
- Analyze the time complexity.
- Learn optimization techniques.

---

# What is Recursion?

Recursion is a programming technique in which a method calls itself repeatedly until a stopping condition (base case) is reached.

It is useful for solving problems that can be divided into smaller subproblems.

---

# Algorithm

Future Value Formula

Future Value = Present Value × (1 + Growth Rate)^Years

Instead of using loops or the `Math.pow()` method, this exercise computes the value recursively.

---

# Base Case

If the number of years is 0, the future value is equal to the present value.

```java
if (years == 0)
    return presentValue;
```

---

# Recursive Case

```java
return (1 + growthRate) *
       calculateFutureValue(presentValue, growthRate, years - 1);
```

---

# Time Complexity

| Case | Complexity |
|------|------------|
| Recursive Solution | O(n) |

where **n** is the number of years.

---

# Optimization

Although this recursive solution has O(n) time complexity, recursion creates additional function call overhead.

Possible optimizations include:

- Iterative solution using a loop
- Dynamic Programming (Memoization)
- Direct mathematical formula using `Math.pow()`

These approaches reduce overhead and improve performance for larger inputs.

---

# Sample Output

```
Present Value : 10000.00
Growth Rate   : 10.00%
Years         : 5
Future Value  : 16105.10
```

---

# Conclusion

Recursion provides a simple and elegant solution for financial forecasting by repeatedly applying the growth rate. However, for very large inputs, iterative or mathematical approaches are generally more efficient due to lower overhead.