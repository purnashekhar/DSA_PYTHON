

# 📘 **ARRAYS — Complete**

## **1. What is an Array?**

An **array** is a collection of elements stored at **continuous memory locations**, accessed using an **index**.

In Python, the closest structure to an array is a **List**.

Example:

```python
arr = [10, 20, 30, 40]
```

---

# **2. Why Arrays Matter in DSA**

* Fast access (O(1) indexing)
* Used in **two pointers**, **prefix sum**, **searching**, **sorting**, **sliding window**
* Most interview problems start with arrays
* Foundation for strings, hashing, stack, queue

---

# **3. Basic Operations (Python List)**

Below are the operations and their time complexity (important in DSA).

### ✔ Access element

```python
arr[i]
```

➡ **O(1)**

### ✔ Update element

```python
arr[i] = 50
```

➡ **O(1)**

---

# **4. List Methods in Python (What You Must Know)**

### ➤ **1. append() — add at end**

```python
arr.append(x)
```

➡ **O(1)** average

### ➤ **2. pop() — remove last element**

```python
arr.pop()
```

➡ **O(1)**

### ➤ **3. insert() — insert at index**

```python
arr.insert(i, x)
```

➡ **O(n)** (shifts elements)

### ➤ **4. remove() — remove by value**

```python
arr.remove(x)
```

➡ **O(n)** (search + shift)

### ➤ **5. del — delete by index**

```python
del arr[i]
```

➡ **O(n)** (shift)

### ➤ **6. slicing**

```python
arr[1:4]
```

➡ **O(k)** where k = slice length

### ➤ **7. length**

```python
len(arr)
```

➡ **O(1)**

---

# **5. How Arrays Work Internally**

* Stored in **continuous blocks of memory**
* Python lists are **dynamic arrays**

  * They grow automatically when needed
  * Expansion uses *amortized O(1)* resizing

This is why `append()` is fast most of the time.

---

# **6. Types of Arrays (Conceptual)**

### ✔ Static Array

* Fixed size
* In languages like C/C++
* Python does NOT have this

### ✔ Dynamic Array (Python List)

* Can grow/shrink
* Real implementation used in Python

---

# **7. Traversing an Array**

Traversing = visiting each element.

### Normal loop:

```python
for x in arr:
    print(x)
```

➡ **O(n)**

### Using index:

```python
for i in range(len(arr)):
    print(arr[i])
```

➡ **O(n)**

---

# **8. Searching in Arrays**

### ➤ **Linear Search**

Check all elements.

```python
for x in arr:
    if x == target:
        return True
```

➡ **O(n)**

### ➤ **Binary Search (only sorted array)**

Divide & conquer.
➡ **O(log n)**

(You will learn this in Searching module.)

---

# **9. Array Memory Indexing**

If array = `[10, 20, 30, 40]`

| Index | Value |
| ----- | ----- |
| 0     | 10    |
| 1     | 20    |
| 2     | 30    |
| 3     | 40    |

Indexing always starts at **0**.

---

# **10. Array Slicing (Important in Python)**

```python
arr[start:end]     # end is non-inclusive
arr[:3]            # first 3 elements
arr[2:]            # from index 2 to end
arr[::-1]          # reverse array
```

Very useful in problems.

---

# **11. Common Array Patterns (Used in DSA)**

These patterns are used in almost **50%** of array problems.

### ✔ Frequency array / Hashmap

Count occurrences of each element.

### ✔ Prefix sum

Fast range queries
`prefix[i] = sum(arr[0..i])`

### ✔ Two pointers

Left & right pointer approach.

### ✔ Sliding window

Fixed-size or variable-size windows for subarray problems.

### ✔ Sorting arrays

For optimum solutions in many problems.

---

# **12. Time Complexities To Memorize**

| Operation          | Big-O          |
| ------------------ | -------------- |
| Access element     | O(1)           |
| Update element     | O(1)           |
| Append at end      | O(1) amortized |
| Insert at index    | O(n)           |
| Delete at index    | O(n)           |
| Loop through array | O(n)           |
| Nested loops       | O(n²)          |

---

# **13. Space Complexity with Arrays**

### ✔ No extra array → O(1)

```python
for i in arr:
```

### ✔ Creating new array → O(n)

```python
new_arr = arr[:]
```

### ✔ Extra prefix/hash arrays → O(n)

---

# **14. When to Use Arrays**

Use arrays when:

* You need fast access
* You need to traverse repeatedly
* Order matters
* Working with numbers, strings, dates, objects

Not ideal when:

* Frequent insertions/deletions in the middle → use deque instead

---

# 🎉 **Arrays — Complete Summary (For Quick Revision)**

* Python list = dynamic array
* Access/update = O(1)
* Insert/delete in middle = O(n)
* append/pop end = O(1)
* Traversing = O(n)
* Used in 80% of DSA basic problems
* Base for two pointers, sliding window, prefix sum, searching & sorting

---


