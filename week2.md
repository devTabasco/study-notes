---
layout: post
title: "Week 2: Algorithms and Complexity"
date: 2024-03-27
categories: computer-science
---

# Algorithms and Complexity

## Understanding Time Complexity

Time complexity is a crucial concept in computer science that helps us analyze and compare the efficiency of different algorithms. It's typically expressed using Big O notation.

### Common Time Complexities

1. O(1) - Constant Time
2. O(log n) - Logarithmic Time
3. O(n) - Linear Time
4. O(n log n) - Linearithmic Time
5. O(n²) - Quadratic Time
6. O(2ⁿ) - Exponential Time

## Sorting Algorithms

### Bubble Sort
```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
    return arr
```

- Time Complexity: O(n²)
- Space Complexity: O(1)
- Stable: Yes

### Quick Sort
```python
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quick_sort(left) + middle + quick_sort(right)
```

- Time Complexity: O(n log n) average, O(n²) worst
- Space Complexity: O(log n)
- Stable: No

## Searching Algorithms

### Binary Search
- Only works on sorted arrays
- Time Complexity: O(log n)
- Space Complexity: O(1)

### Linear Search
- Works on any array
- Time Complexity: O(n)
- Space Complexity: O(1)

## Practice Problems

1. Implement Merge Sort
2. Find the kth largest element in an unsorted array
3. Implement Binary Search recursively and iteratively

## Additional Resources

- [Introduction to Algorithms (CLRS)](https://mitpress.mit.edu/books/introduction-algorithms-fourth-edition)
- [Visualizing Algorithms](https://visualgo.net/en/sorting) 