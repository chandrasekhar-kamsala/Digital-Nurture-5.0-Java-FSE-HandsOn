# Exercise 2: E-commerce Platform Search Function

## Scenario

You are working on the search functionality of an e-commerce platform. The search needs to be optimized for fast performance.

---

## Objective

- Understand Big O Notation.
- Explain Best, Average and Worst Case.
- Implement Linear Search.
- Implement Binary Search.
- Compare the performance of both algorithms.

---

# Big O Notation

Big O Notation is used to measure the efficiency of an algorithm. It describes how the execution time or memory usage grows as the input size increases.

It helps developers compare algorithms and choose the most efficient one for a given problem.

---

# Search Operation Analysis

## Best Case

The required product is found in the first comparison.

Time Complexity

- Linear Search : O(1)
- Binary Search : O(1)

---

## Average Case

The required product is found somewhere in the middle.

Time Complexity

- Linear Search : O(n)
- Binary Search : O(log n)

---

## Worst Case

The required product is the last element or is not present.

Time Complexity

- Linear Search : O(n)
- Binary Search : O(log n)

---

# Project Structure

```
Exercise-02-Ecommerce-Platform-Search-Function
│
├── README.md
└── src
    ├── Product.java
    ├── LinearSearch.java
    ├── BinarySearch.java
    └── EcommerceSearch.java
```

---

# Classes Used

## Product.java

Represents the product with the following attributes:

- Product ID
- Product Name
- Category

---

## LinearSearch.java

Implements the Linear Search algorithm.

Characteristics:

- Works on unsorted data.
- Checks each product one by one.
- Time Complexity: O(n)

---

## BinarySearch.java

Implements the Binary Search algorithm.

Characteristics:

- Works only on sorted data.
- Repeatedly divides the search space into two halves.
- Time Complexity: O(log n)

---

## EcommerceSearch.java

Driver class that creates sample products and demonstrates both Linear Search and Binary Search.

---

# Sample Products

| Product ID | Product Name | Category |
|------------|--------------|----------|
|101|Laptop|Electronics|
|102|Mobile|Electronics|
|103|Shoes|Fashion|
|104|Watch|Accessories|
|105|Book|Education|

---

# Sample Output

```
========== LINEAR SEARCH ==========
Product ID : 104
Product Name : Watch
Category : Accessories

========== BINARY SEARCH ==========
Product ID : 104
Product Name : Watch
Category : Accessories
```

---

# Time Complexity Comparison

| Algorithm | Best | Average | Worst |
|-----------|------|----------|--------|
| Linear Search | O(1) | O(n) | O(n) |
| Binary Search | O(1) | O(log n) | O(log n) |

---

# Comparison

## Linear Search

Advantages

- Simple to implement.
- Works on both sorted and unsorted data.

Disadvantages

- Slow for large datasets.

---

## Binary Search

Advantages

- Very fast.
- Efficient for large datasets.

Disadvantages

- Requires sorted data.

---

# Conclusion

For an e-commerce platform containing thousands or millions of products, Binary Search is more suitable because it performs searches in O(log n) time, making it significantly faster than Linear Search for large datasets.