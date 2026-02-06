# 📘 DSA Notes – Abdul Bari (Clean Reference Version)

This document provides a **clear, structured, and interview‑ready reference** for understanding Algorithms, Time Complexity, Space Complexity, and Matrix Multiplication analysis.

---

# 📖 Table of Contents

* What is an Algorithm?
* What is a Program?
* Algorithm vs Program
* Priori vs Posteriori Analysis
* Characteristics of an Algorithm
* How to Write an Algorithm
* Time and Space Complexity
* Frequency Count Method
* Matrix Addition Complexity
* Matrix Multiplication Complexity
* Time Complexity Patterns
* Complexity Reference Table
* Key Takeaways

---

# 🧠 What is an Algorithm?

An **algorithm** is a step‑by‑step procedure used to solve a problem.

### Key points:

* Logical sequence of steps
* Language independent
* Focuses on solution design

Example:

```
Algorithm Swap(a, b)
Begin
    temp = a
    a = b
    b = temp
End
```

---

# 💻 What is a Program?

A **program** is the implementation of an algorithm using a programming language.

Example languages:

* Java
* Python
* C
* C++

Program is:

* Executable
* Language dependent
* Hardware dependent

---

# ⚖️ Algorithm vs Program

| Algorithm               | Program                        |
| ----------------------- | ------------------------------ |
| Design                  | Implementation                 |
| Language independent    | Language dependent             |
| Hardware independent    | Hardware dependent             |
| Cannot execute directly | Executable                     |
| Used for analysis       | Used for solving real problems |

---

# 📊 Priori vs Posteriori Analysis

## Priori Analysis

Done before implementation.

Based on:

* Mathematical analysis
* Independent of hardware

Example:

```
f(n) = n²
```

---

## Posteriori Analysis

Done after implementation.

Based on:

* Actual execution time
* Actual memory usage

Depends on:

* Hardware
* Programming language

---

# ✅ Characteristics of an Algorithm

An algorithm must have:

## 1. Input

Zero or more inputs

## 2. Output

At least one output

## 3. Definiteness

Each step must be clear

## 4. Finiteness

Must terminate

## 5. Effectiveness

Must be efficient and practical

---

# ✍️ How to Write an Algorithm

Example: Swap two numbers

```
Algorithm Swap(a, b)
Begin
    temp = a
    a = b
    b = temp
End
```

---

# ⏱️ Time Complexity

Time complexity measures how execution time increases with input size.

Example:

```
temp = a
a = b
b = temp
```

Time function:

```
f(n) = 3
O(1)
```

Constant time.

---

# 💾 Space Complexity

Space complexity measures memory usage.

Example swap uses:

```
a, b, temp
```

Space:

```
O(1)
```

---

# 🔢 Frequency Count Method

Counts exact number of operations.

Example: Sum of array

```
Algorithm Sum(A, n)
Begin
    sum = 0
    for i = 0 to n-1
        sum = sum + A[i]
    return sum
End
```

Time function:

```
f(n) = 2n + 3
```

Big‑O:

```
O(n)
```

Space:

```
O(n)
```

---

# 🧮 Matrix Addition Complexity

Algorithm:

```
for i = 0 to n-1
  for j = 0 to n-1
    C[i][j] = A[i][j] + B[i][j]
```

Time complexity:

```
O(n²)
```

Space complexity:

```
O(n²)
```

---

# 🧮 Matrix Multiplication Complexity

Multiply two matrices A and B of size n × n.

## Algorithm

```
Algorithm Multiply(A, B, n)
Begin
    for i = 0 to n-1
        for j = 0 to n-1
            C[i][j] = 0
            for k = 0 to n-1
                C[i][j] = C[i][j] + A[i][k] * B[k][j]
End
```

---

## Time Complexity

Loop execution count:

```
i loop = n
j loop = n
k loop = n
```

Total operations:

```
n × n × n
= n³
```

Final:

```
O(n³)
```

---

## Space Complexity

Matrices used:

```
A = n²
B = n²
C = n²
```

Final:

```
O(n²)
```

---

# 📈 Time Complexity Patterns

## Linear Time — O(n)

Example:

```
for i = 0 to n-1
```

---

## Quadratic Time — O(n²)

Example:

```
for i = 0 to n-1
  for j = 0 to n-1
```

---

## Cubic Time — O(n³)

Example:

Matrix multiplication

---

## Square Root Time — O(√n)

Example:

```
p = 0
for i = 1 while p <= n
  p = p + i
```

Complexity:

```
O(√n)
```

---

# 📊 Complexity Reference Table

| Complexity | Name         | Example               |
| ---------- | ------------ | --------------------- |
| O(1)       | Constant     | Variable swap         |
| O(log n)   | Logarithmic  | Binary search         |
| O(n)       | Linear       | Single loop           |
| O(n log n) | Linearithmic | Merge sort            |
| O(n²)      | Quadratic    | Nested loops          |
| O(n³)      | Cubic        | Matrix multiplication |
| O(2ⁿ)      | Exponential  | Recursive Fibonacci   |

---

# 🎯 Key Takeaways

* Algorithm is design
* Program is implementation
* Time complexity measures speed
* Space complexity measures memory
* Nested loops multiply complexity
* Focus on highest power of n

---

# 📚 Credits

Based on Abdul Bari DSA lectures

---

# ⭐ Recommended Usage

Use this document as:

* Interview preparation reference
* DSA fundamentals revision
* Complexity analysis reference
* Algorithm design guide

---

**End of Document**
