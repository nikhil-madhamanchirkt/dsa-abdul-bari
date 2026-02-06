# 📘 DSA Notes – Abdul Bari

This repository contains structured notes on **Data Structures and Algorithms (DSA)** based on Abdul Bari's lectures. These notes cover fundamental concepts such as algorithms, program analysis, time and space complexity, and algorithm characteristics.

---

# 📖 Table of Contents

* [What is an Algorithm?](#-what-is-an-algorithm)
* [What is a Program?](#-what-is-a-program)
* [Algorithm vs Program](#-algorithm-vs-program)
* [Priori vs Posteriori Analysis](#-priori-vs-posteriori-analysis)
* [Characteristics of an Algorithm](#-characteristics-of-an-algorithm)
* [How to Write an Algorithm](#-how-to-write-an-algorithm)
* [How to Analyze an Algorithm](#-how-to-analyze-an-algorithm)
* [Frequency Count Method](#-frequency-count-method)
* [Examples](#-examples)

---

# 🧠 What is an Algorithm?

An **algorithm** is a step‑by‑step procedure for solving a computational problem.

It is:

* A logical sequence of steps
* Independent of programming language
* Focused on problem-solving approach

---

# 💻 What is a Program?

A **program** is the implementation of an algorithm using a programming language such as Java, C, or Python.

It is:

* Executable by a computer
* Dependent on hardware and operating system

---

# ⚖️ Algorithm vs Program

| Algorithm                        | Program                        |
| -------------------------------- | ------------------------------ |
| Design phase                     | Implementation phase           |
| Written by designer or architect | Written by programmer          |
| Language independent             | Language dependent             |
| Hardware independent             | Hardware dependent             |
| Used for analysis                | Used for execution and testing |

---

# 📊 Priori vs Posteriori Analysis

| Priori Analysis                       | Posteriori Analysis             |
| ------------------------------------- | ------------------------------- |
| Done on algorithm                     | Done on program                 |
| Independent of language               | Language dependent              |
| Hardware independent                  | Hardware dependent              |
| Uses mathematical functions           | Uses actual execution metrics   |
| Measures time and space theoretically | Measures actual time and memory |

---

# ✅ Characteristics of an Algorithm

An algorithm must have the following properties:

### 1. Input

* Zero or more inputs

### 2. Output

* At least one output

### 3. Definiteness

* Each step must be clear and unambiguous

### 4. Finiteness

* Must terminate after finite number of steps

### 5. Effectiveness

* Must be simple, practical, and executable

---

# ✍️ How to Write an Algorithm

Example: Swap two numbers

```text
Algorithm Swap(a, b)
Begin
    temp ← a
    a ← b
    b ← temp
End
```

---

# 🔍 How to Analyze an Algorithm

Algorithm analysis measures resource usage.

### Resources measured:

1. Time complexity
2. Space complexity
3. Network usage
4. Power consumption
5. CPU usage

---

# ⏱️ Time Complexity Example

Swap algorithm:

```text
temp = a
 a = b
 b = temp
```

Time function:

```
f(n) = 3
O(1) → Constant Time
```

---

# 💾 Space Complexity Example

Variables used:

* a
* b
* temp

```
S(n) = 3
O(1) → Constant Space
```

---

# 🔢 Frequency Count Method

Used to calculate exact number of operations.

Example: Sum of array

```text
Algorithm Sum(A, n)
Begin
    s ← 0
    for i ← 0 to n-1
        s ← s + A[i]
    return s
End
```

### Time Complexity

```
f(n) = 2n + 3
O(n)
```

### Space Complexity

```
S(n) = n + 3
O(n)
```

---

# 🧮 Matrix Addition Example

Add two matrices of size n × n

```text
Algorithm Add(A, B, n)
Begin
    for i ← 0 to n-1
        for j ← 0 to n-1
            C[i][j] ← A[i][j] + B[i][j]
End
```

### Time Complexity

```
f(n) = 2n² + 2n + 1
O(n²)
```

### Space Complexity

```
S(n) = 3n² + 3
O(n²)
```

---

# 🎯 Key Complexity Classes

| Complexity | Name         | Example              |
| ---------- | ------------ | -------------------- |
| O(1)       | Constant     | Access array element |
| O(log n)   | Logarithmic  | Binary Search        |
| O(n)       | Linear       | Loop through array   |
| O(n log n) | Linearithmic | Merge Sort           |
| O(n²)      | Quadratic    | Nested loops         |
| O(2ⁿ)      | Exponential  | Recursive Fibonacci  |

---

# 🚀 Summary

* Algorithm is the design
* Program is the implementation
* Time complexity measures speed
* Space complexity measures memory
* Frequency count gives exact analysis
* Big‑O gives growth rate

---

Matrix Multiplication Time and Space Complexity
Problem

Multiply two matrices A and B of size n × n to produce matrix C.

Algorithm
Algorithm multiply(A, B, n)
Begin
  for i = 0 to n-1
    for j = 0 to n-1
      C[i][j] = 0
      for k = 0 to n-1
        C[i][j] = C[i][j] + A[i][k] * B[k][j]
End
Time Complexity Analysis (Frequency Count Method)
Loop Execution Count
Loop	Runs	Explanation
i loop	n	iterates over rows
j loop	n	iterates over columns
k loop	n	performs multiplication and addition
Total execution count
Total operations = n × n × n
                 = n³
Mathematical Function
f(n) = n³
Big‑O Notation
O(n³)
Space Complexity Analysis
Variables Used
Variable	Space Required
Matrix A	n²
Matrix B	n²
Matrix C	n²
i, j, k	3
Total Space
s(n) = 3n² + 3
Big‑O Space
O(n²)
Time Complexity Analysis Notes

These notes help analyze algorithm complexity based on loop structures.

1. Linear Time Complexity — O(n)
Simple Loop
for(i = 1; i <= n; i++)

Runs n times

Time Complexity = O(n)
Reverse Loop
for(i = n; i >= 1; i--)

Also runs n times

Time Complexity = O(n)
Loop with Step Increment
for(i = 1; i <= n; i = i + 2)

Runs n/2 times

But Big‑O ignores constants:

O(n)

Example:

n/20 → O(n)
2. Quadratic Time Complexity — O(n²)
Standard Nested Loop
for(i = 0; i < n; i++)
  for(j = 0; j < n; j++)

Execution count:

n × n = n²
O(n²)
Dependent Nested Loop
for(i = 0; i < n; i++)
  for(j = 0; j < i; j++)

Execution pattern:

When i = 0 → 0 times
When i = 1 → 1 time
When i = 2 → 2 times
...
When i = n → n times

Total executions:

1 + 2 + 3 + ... + n
= n(n+1)/2

Polynomial form:

(n² + n)/2

Ignoring lower term:

O(n²)
3. Square Root Time Complexity — O(√n)
Example
p = 0
for(i = 1; p <= n; i++)
  p = p + i

Execution pattern:

p = 1 + 2 + 3 + ... + k

Formula:

p = k(k+1)/2

Condition:

k² ≈ n

Result:

k ≈ √n

Time complexity:

O(√n)
Key Takeaways for Complexity Analysis
1. Tracing Method

Track variable values step‑by‑step.

Example:

i = 1, 2, 3, 4, ..., n

Count total executions.

2. Frequency Count Method

Count how many times each statement executes.

Example:

for(i=0; i<n; i++)

Runs n times.

3. Focus on Highest Degree

Example:

f(n) = n² + n + 10

Ignore lower terms:

O(n²)
4. Ignore Constants

Example:

f(n) = 5n + 10

Result:

O(n)
5. Common Complexity Reference Table
Complexity	Name	Example
O(1)	Constant	Access array element
O(log n)	Logarithmic	Binary search
O(n)	Linear	Simple loop
O(n log n)	Linearithmic	Merge sort
O(n²)	Quadratic	Nested loops
O(n³)	Cubic	Matrix multiplication
O(2ⁿ)	Exponential	Recursive Fibonacci
Matrix Multiplication Summary
Metric	Complexity
Time Complexity	O(n³)
Space Complexity	O(n²)
Type	Cubic time algorithm

Author: Abdul Bari DSA Notes (Refined and Structured)

# 📚 Credits

Based on lectures by **Abdul Bari**

---

# ⭐ Support

If you find this helpful, please ⭐ this repository.
