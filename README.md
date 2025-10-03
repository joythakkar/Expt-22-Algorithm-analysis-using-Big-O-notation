
## Title  
**Algorithm Analysis using Big O Notation**  

---

## Aim  
To study and analyze the efficiency of algorithms using **Big O Notation** and to understand how different algorithms behave with respect to input size in terms of time and space requirements.  

---

## Objectives  
1. To understand the importance of algorithm analysis in computer science.  
2. To study the concept of **time complexity** and **space complexity**.  
3. To understand the role of **asymptotic notations** (Big O, Big Ω, Big Θ).  
4. To analyze algorithms in terms of **best-case, worst-case, and average-case scenarios**.  
5. To compare the growth rates of commonly used algorithms.  
6. To learn how algorithm efficiency affects performance on large datasets.  

---

## Theory  

### 1. Introduction to Algorithm Analysis  
An **algorithm** is a step-by-step procedure to solve a problem. While multiple algorithms may exist for the same problem, their **efficiency** can differ drastically. An inefficient algorithm may work for small input sizes, but fail for large-scale problems.  

Hence, it is crucial to analyze algorithms before implementation to ensure they can handle large inputs effectively.  

Algorithm analysis focuses on:  
- **Time Complexity**: How fast the algorithm executes.  
- **Space Complexity**: How much memory the algorithm consumes.  

---

### 2. Why Do We Need Big O Notation?  
- The execution time of a program depends on CPU speed, compiler optimizations, and system load, making exact measurement unreliable.  
- Instead of exact time, we use **growth functions** that show how the number of operations increases with input size `n`.  
- **Big O Notation** provides a **machine-independent, generalized measure** of efficiency.  

---

### 3. Types of Algorithmic Complexity  

#### a) Time Complexity  
It refers to the amount of **CPU time** an algorithm requires. Examples:  
- **Linear Search:** Takes O(n) time because it checks each element once.  
- **Binary Search:** Takes O(log n) time because it halves the search space each step.  
- **Bubble Sort:** Takes O(n²) time because of nested loops.  
- **Merge Sort:** Takes O(n log n) time because of recursive division.  

#### b) Space Complexity  
It refers to the **memory required** by the algorithm during execution.  
Components:  
- Fixed part (instructions, constants).  
- Variable part (input data, recursion stack, auxiliary storage).  

Example:  
- Iterative algorithms → low space complexity.  
- Recursive algorithms (like Quick Sort) → higher space complexity due to function stack.  

---

### 4. Asymptotic Notations  

1. **Big O (O):** Upper bound – worst case.  
   Example: Binary Search → O(log n).  

2. **Big Ω (Ω):** Lower bound – best case.  
   Example: Linear Search best case (element at first index) → Ω(1).  

3. **Big Θ (Θ):** Tight bound – average case.  
   Example: Bubble Sort → Θ(n²).  

---

### 5. Growth Rate of Functions  
Growth rate describes how running time increases with input size.  

- **O(1) Constant Time:** Example: Accessing `arr[i]`.  
- **O(log n) Logarithmic:** Example: Binary Search.  
- **O(n) Linear:** Example: Linear Search.  
- **O(n log n):** Example: Merge Sort, Quick Sort.  
- **O(n²):** Example: Bubble Sort, Selection Sort.  
- **O(2ⁿ):** Example: Recursive Fibonacci.  
- **O(n!):** Example: Traveling Salesman Problem.  

---

### 6. Best, Average, and Worst Case  

- **Best Case (Ω):** Minimum operations. Example: Linear Search finds element at first position → O(1).  
- **Average Case (Θ):** Expected performance on random inputs. Example: Searching for an element in the middle → O(n/2) ≈ O(n).  
- **Worst Case (O):** Maximum operations. Example: Linear Search where element is not found → O(n).  

---

## Comparison Table of Common Complexities  

| Complexity | Name             | Example Algorithms                  | Growth Rate (n=10) | Growth Rate (n=100) | Growth Rate (n=1000) |
|------------|------------------|--------------------------------------|--------------------|---------------------|-----------------------|
| O(1)       | Constant         | Array element access                 | 1                  | 1                   | 1                     |
| O(log n)   | Logarithmic      | Binary Search                        | 3                  | 7                   | 10                    |
| O(n)       | Linear           | Linear Search                        | 10                 | 100                 | 1000                  |
| O(n log n) | Linearithmic     | Merge Sort, Quick Sort (avg)         | 30                 | 700                 | 10000                 |
| O(n²)      | Quadratic        | Bubble Sort, Selection Sort          | 100                | 10,000              | 1,000,000             |
| O(2ⁿ)      | Exponential      | Recursive Fibonacci, Subset Problem  | 1024               | Huge                | Extremely Huge        |

---

## Program Summary  

In this experiment, various algorithms were studied to understand their time complexities:  

1. **Linear Search** → O(n)  
   - Works by scanning each element one by one.  
   - Simple but inefficient for large datasets.  

2. **Binary Search** → O(log n)  
   - Works on sorted arrays by repeatedly dividing the search space.  
   - Much faster than linear search.  

3. **Bubble Sort** → O(n²)  
   - Repeatedly swaps adjacent elements until sorted.  
   - Easy to implement but slow.  

4. **Quick Sort** → O(n log n) average case, O(n²) worst case  
   - Efficient sorting algorithm using divide-and-conquer.  
   - Performs well in practice.  

---

## Algorithm (General Steps for Big O Analysis)  

1. Define the **input size (n)**.  
2. Identify the **basic operation(s)** (comparison, swap, addition).  
3. Count how many times the basic operation is executed for input `n`.  
4. Express the function in terms of `n`.  
5. Drop constants and lower-order terms.  
6. Express the result in **asymptotic notation**.  

---

## Concepts Used  
- Algorithm design and efficiency.  
- Time and space complexity.  
- Asymptotic notations (Big O, Big Ω, Big Θ).  
- Best-case, worst-case, average-case analysis.  
- Growth rate comparison of common algorithms.  
- Recursive vs iterative approaches.  

---

## Conclusion  

1. Big O Notation provides a **standard mathematical model** to describe algorithm performance.  
2. It abstracts away hardware and focuses only on **growth with input size**.  
3. Algorithms with lower complexity like **O(log n)** (Binary Search) are highly efficient compared to **O(n²)** (Bubble Sort).  
4. **Efficient algorithms** are necessary for scalability in real-world applications like databases, search engines, and networking.  
5. Understanding time and space trade-offs helps programmers design **optimal solutions**.  
6. Thus, analyzing algorithms using Big O Notation is **essential for computer scientists and engineers** to make informed choices when solving problems.  

---
