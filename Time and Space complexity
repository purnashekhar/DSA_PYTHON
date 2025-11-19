
# 📘 **Big-O Notation — Complete Notes**

## **1. What is Big-O?**

Big-O notation describes **how the running time or space usage of an algorithm grows** as the **input size (n)** increases.

It does **not** measure:

* exact time
* hardware speed
* programming language differences

It measures the **growth rate** of your algorithm.

---

## **2. Why Big-O Matters for Data Analysts**

* Helps you write efficient Python code for large datasets.
* Helps you understand which operations explode in time (O(n²)).
* Helps you evaluate SQL, Python loops, transformations, and ETL steps.
* Great for analytics interviews & problem-solving.

---

# **3. Common Big-O Complexities (Only the Ones You Need)**

## ✔ **O(1) — Constant Time**

Time does **not** depend on input size.

### Example

```python
x = arr[0]  # accessing index
```

### Notes

* Fastest possible
* Dictionary lookup, set lookup are avg O(1)

---

## ✔ **O(n) — Linear Time**

Time grows **linearly** with input size.

### Example

```python
for x in arr:
    print(x)
```

### Notes

* One full scan
* Most data cleaning steps in Pandas are O(n)

---

## ✔ **O(n²) — Quadratic Time**

Nested loops → very slow for large datasets.

### Example

```python
for i in arr:
    for j in arr:
        pass
```

### Notes

* Avoid on large data
* Comparing every row with every other row

---

## ✔ **O(log n) — Logarithmic Time**

Reduces work by **half** each time.

### Example

```python
# Binary Search
```

### Notes

* Searching in ordered data
* SQL index lookups are O(log n)

---

## ✔ **O(n log n) — Linearithmic Time**

Used by sorting algorithms.

### Example

```python
arr.sort()
```

### Notes

* Sorting is heavy
* Python’s built-in sort is O(n log n)

---

# **4. Time Complexity Patterns**

### **Single loop**

```python
for i in arr:
```

➡ **O(n)**

### **Nested loops**

```python
for i in arr:
    for j in arr:
```

➡ **O(n²)**

### **Loop + constant work**

```python
for i in arr:
    x = 10
```

➡ **O(n)**

### **Early break**

```python
for x in arr:
    if x == target:
        break
```

➡ **Still O(n)** (worst-case)

---

# **5. Space Complexity (Basics Only)**

## ✔ **O(1) Space**

No new significant data structures.

```python
sum = 0
```

## ✔ **O(n) Space**

You create a list, dict, set of size n.

```python
new_arr = arr[:]  
```

## ✔ **Recursion adds stack space**

```python
def f(n):
    return f(n-1)
```

➡ space = depth of recursion

---

# **6. Summary Chart**

| Complexity     | Meaning     | Example           |
| -------------- | ----------- | ----------------- |
| **O(1)**       | Constant    | Accessing element |
| **O(log n)**   | Logarithmic | Binary Search     |
| **O(n)**       | Linear      | Loop through list |
| **O(n log n)** | Log-linear  | Sorting           |
| **O(n²)**      | Quadratic   | Nested loops      |

---

# **7. Real-World Data Analyst Examples**

### ✔ Scanning all rows

➡ O(n)

### ✔ Finding duplicates using a set

➡ O(n)

### ✔ Sorting a sales table

➡ O(n log n)

### ✔ Cross-join style operations

➡ O(n²)

### ✔ SQL indexed search

➡ O(log n)

### ✔ GroupBy in Pandas

➡ O(n)

---

# **8. Ultra-Short Summary for Interviews**

* Loops → **O(n)**
* Nested loops → **O(n²)**
* Sorting → **O(n log n)**
* Hashing → **O(1)** avg
* Binary search → **O(log n)**
* Recursion → depends, but add stack space
* Choose O(n) or lower whenever possible

