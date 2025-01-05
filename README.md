# Data Structures and Algorithms in Python & JavaScript

Welcome to this repository of **Data Structures and Algorithms** implemented in both **Python** and **JavaScript**. Whether you're a beginner trying to grasp the basics or an experienced developer looking to sharpen your problem-solving skills, this repository is designed to provide clear, easy-to-understand examples of important data structures and algorithms.

The purpose of this repository is to provide useful code implementations for common data structures and algorithms, with both **Python** and **JavaScript** versions available for comparison. This can be a valuable resource for preparing for technical interviews, practicing coding challenges, or simply expanding your knowledge.

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Data Structures](#data-structures)
  - [Arrays](#arrays)
  - [Linked Lists](#linked-lists)
  - [Stacks](#stacks)
  - [Queues](#queues)
  - [Hash Tables](#hash-tables)
  - [Trees](#trees)
  - [Graphs](#graphs)
- [Algorithms](#algorithms)
  - [Sorting](#sorting)
  - [Searching](#searching)
  - [Dynamic Programming](#dynamic-programming)
  - [Greedy Algorithms](#greedy-algorithms)
  - [Graph Algorithms](#graph-algorithms)
- [How to Use](#how-to-use)
- [Examples](#examples)
- [Challenges](#challenges)
- [Resources](#resources)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository contains code for commonly used **data structures** and **algorithms**. Each algorithm and data structure is implemented in both **Python** and **JavaScript**, so you can compare the syntax and approaches in both languages. The goal is to provide clear and understandable code that you can use to learn, practice, and solve problems efficiently.

### Key Features:
- **Data Structures**: Arrays, Linked Lists, Stacks, Queues, Hash Tables, Trees, Graphs.
- **Algorithms**: Sorting, Searching, Dynamic Programming, Greedy Algorithms, Graph Algorithms.
- **Two Language Implementations**: All algorithms and data structures are implemented in both Python and JavaScript for easy comparison.

## Getting Started

Follow these steps to set up the repository and start experimenting with the code on your local machine.

### Prerequisites

Before running the code, you need to have the following installed:

- **Python 3.x**: [Download Python](https://www.python.org/downloads/)
- **Node.js**: [Download Node.js](https://nodejs.org/en/)

### Clone the Repository

Clone this repository to your local machine using Git:

```bash
git clone https://github.com/thatritikpatel/DSA-with-Python-and-Javascript.git
```

### Python Setup

1. Navigate to the `python/` directory.
2. If there are any dependencies (such as for a specific algorithm or visualization), install them by running:

```bash
pip install -r requirements.txt
```

### JavaScript Setup

1. Navigate to the `javascript/` directory.
2. Install dependencies (if applicable) by running:

```bash
npm install
```

## Data Structures

Here are the core data structures included in this repository:

### Arrays

Arrays are a collection of elements stored in a contiguous block of memory. Each element is accessed by an index.

- **Operations**: Access, insertion, deletion, and searching by index.
- **Applications**: Arrays are commonly used for storing lists of items, implementing hash tables, and representing matrices.

### Linked Lists

A linked list is a linear collection of elements, where each element (node) points to the next element. It provides efficient insertions and deletions but slower access times for random access.

- **Types**: 
  - **Singly Linked List**: Each node points to the next node.
  - **Doubly Linked List**: Each node points to both the next and previous nodes.
  - **Circular Linked List**: The last node points back to the first node.

### Stacks

A stack is a data structure that follows the Last-In-First-Out (LIFO) principle. The last element added is the first one to be removed.

- **Operations**: `push` (add item), `pop` (remove item), and `peek` (view top item).
- **Applications**: Undo functionality, recursion handling, depth-first search (DFS).

### Queues

A queue is a data structure that follows the First-In-First-Out (FIFO) principle. The first element added is the first one to be removed.

- **Operations**: `enqueue` (add item), `dequeue` (remove item).
- **Applications**: Task scheduling, breadth-first search (BFS), handling asynchronous requests.

### Hash Tables

Hash tables store key-value pairs and use a hash function to map the keys to specific locations in memory. This allows for efficient lookup, insertion, and deletion.

- **Operations**: Insertion, deletion, and search by key.
- **Applications**: Caching, counting frequencies, associative arrays.

### Trees

A tree is a hierarchical data structure with nodes connected by edges. Trees are essential in many areas of computer science, such as search algorithms, file systems, and databases.

- **Types**:
  - **Binary Tree**: Each node has at most two children.
  - **Binary Search Tree**: A binary tree with a specific ordering property.
  - **AVL Tree**: A self-balancing binary search tree.
  - **Heap**: A special tree-based structure used for efficient sorting and priority queue implementation.

### Graphs

A graph is a collection of nodes (vertices) connected by edges. Graphs are useful for modeling networks, social media connections, and much more.

- **Types**:
  - **Directed Graph**: Edges have a direction.
  - **Undirected Graph**: Edges have no direction.
  - **Weighted Graph**: Edges have weights.
- **Applications**: Social networks, web page links, network routing.

## Algorithms

### Sorting Algorithms

Sorting algorithms arrange elements in a specific order, usually ascending or descending. Common algorithms include:

- **Bubble Sort**: A simple comparison-based algorithm, inefficient for large datasets.
- **Quick Sort**: A divide-and-conquer algorithm, generally faster than bubble sort.
- **Merge Sort**: A divide-and-conquer algorithm that guarantees O(n log n) performance.
- **Insertion Sort**: Builds a sorted sequence one element at a time.
- **Selection Sort**: Repeatedly selects the smallest (or largest) element and places it in the correct position.

### Searching Algorithms

Searching algorithms allow you to find an element in a collection:

- **Linear Search**: Searches each element in sequence.
- **Binary Search**: A faster search method for sorted datasets, dividing the search interval in half with each comparison.

### Dynamic Programming

Dynamic programming is a technique for solving complex problems by breaking them into simpler subproblems. It is particularly useful when solving problems that involve overlapping subproblems.

- Examples include the Fibonacci sequence, knapsack problem, and longest common subsequence.

### Greedy Algorithms

Greedy algorithms make locally optimal choices in the hope of finding a global optimum. These algorithms are often faster but may not always produce the best solution.

- Examples include the fractional knapsack problem and activity selection problem.

### Graph Algorithms

Graph algorithms are essential for solving problems related to graph theory:

- **Depth-First Search (DFS)**: Explores as far as possible along each branch before backtracking.
- **Breadth-First Search (BFS)**: Explores all neighbors at the present depth level before moving on to the next depth level.
- **Dijkstra’s Algorithm**: Finds the shortest path from a source node to all other nodes in a weighted graph.

## How to Use

To run any of the data structures or algorithms:

### Python

1. Navigate to the appropriate directory (e.g., `python/sorting/`).
2. Run the script using Python:

```bash
python sort.py
```

### JavaScript

1. Navigate to the appropriate directory (e.g., `javascript/sorting/`).
2. Run the script using Node.js:

```bash
node sort.js
```

You can modify the code to test different inputs or algorithms, or even add your own implementations.

## Examples

### Example 1: Binary Search in Python

```python
def binary_search(arr, target):
    low, high = 0, len(arr) - 1
    while low <= high:
        mid = (low + high) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return -1

arr = [1, 3, 5, 7, 9]
target = 5
result = binary_search(arr, target)
print(f"Element found at index {result}" if result != -1 else "Element not found")
```

### Example 2: Queue Implementation in JavaScript

```javascript
class Queue {
    constructor() {
        this.items = [];
    }
    enqueue(element) {
        this.items.push(element);
    }
    dequeue() {
        if (this.isEmpty()) return "Queue is empty";
        return this.items.shift();
    }
    isEmpty() {
        return this.items.length === 0;
    }
}

let queue = new Queue();
queue.enqueue(1);
queue.enqueue(2);

console.log(queue.dequeue()); // 1
console.log(queue.dequeue()); // 2
```

## Challenges

Here are some challenges to test your understanding:

- Implement a **priority queue**.
- Solve the **knapsack problem** using dynamic programming.
- Create a function to **check for balanced parentheses** using a stack.
- Implement **Dijkstra's algorithm** to find the shortest path in a graph.

## Resources

Here are some great resources to continue learning about data structures and algorithms:

- [GeeksforGeeks](https://www.geeksforgeeks.org/)
- [LeetCode](https://leetcode.com/)
- [HackerRank](https://www.hackerrank.com/)
- [Big-O Cheat Sheet](https://www.bigocheatsheet.com/)

## Contributing

We welcome contributions! If you'd like to add new features, fix bugs, or improve existing implementations, feel free to fork the repository and submit a pull request.

### How to Contribute

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes.
4. Test your changes to ensure everything works.
5. Submit a pull request with a clear explanation of your changes.

## License

This repository is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---

Happy coding! ✨


## Contact
- Ritik Patel - [https://www.linkedin.com/in/thatritikpatel/]
