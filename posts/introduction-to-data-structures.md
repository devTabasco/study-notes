# Introduction to Data Structures

## What are Data Structures?

Data structures are specialized formats for organizing, processing, retrieving and storing data. Understanding data structures is crucial for writing efficient code and solving complex programming problems.

## Basic Data Structures

### 1. Arrays
- Sequential collection of elements
- Fixed size in most languages
- O(1) access time
- Examples and use cases

### 2. Linked Lists
- Dynamic size
- Non-contiguous memory allocation
- O(n) access time
- Singly vs Doubly linked lists

### 3. Stacks
- LIFO (Last In, First Out)
- Common operations: push, pop
- Real-world applications

### 4. Queues
- FIFO (First In, First Out)
- Common operations: enqueue, dequeue
- Priority queues

## Code Examples

```python
# Example of implementing a stack in Python
class Stack:
    def __init__(self):
        self.items = []
    
    def push(self, item):
        self.items.append(item)
    
    def pop(self):
        return self.items.pop()
    
    def is_empty(self):
        return len(self.items) == 0
```

## Practice Problems

1. Implement a queue using two stacks
2. Reverse a linked list
3. Find the middle element of a linked list

## Additional Resources

- [GeeksforGeeks Data Structures](https://www.geeksforgeeks.org/data-structures/)
- [Visualgo - Data Structure Visualization](https://visualgo.net/) 