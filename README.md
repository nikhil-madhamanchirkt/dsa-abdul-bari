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

# 📚 Credits

Based on lectures by **Abdul Bari**

---

# ⭐ Support

If you find this helpful, please ⭐ this repository.
