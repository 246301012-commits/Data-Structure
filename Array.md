📘 Arrays in C – Complete Guide

## 🔹 1. What is an Array?

An **array** is a data structure that stores a collection of **elements of the same type** in **contiguous memory locations**.
This makes it possible to access elements using an **index** efficiently.

```c
int arr[5];   // declaration of array of 5 integers
```

---

## 🔹 2. Why Contiguous Memory Matters

* Elements are stored **sequentially** in memory.
* Address of an element is computed as:

  ```
  base_address + index × size_of_element
  ```
* Benefits:

  * **O(1) random access**
  * **Cache friendly** due to spatial locality

---

## 🔹 3. Key Terminology

* **Indexing** → Zero-based (first element is `arr[0]`)
* **Element** → Value stored at a specific index
* **Length/Size** → Number of items the array can hold

---

## 🔹 4. Declaring and Initializing

```c
int arr[5];                 // Declaration
int arr2[] = {1, 2, 3, 4};  // Initialization with inferred size
```

If fewer values are given, remaining elements are set to `0`.

---

## 🔹 5. Access and Modify Elements

```c
arr[0] = 10;               // Modify
printf("%d", arr[2]);      // Access element
```

In C, the array name acts as a **pointer** to the first element.
So `arr[i]` is equivalent to `*(arr + i)`.

---

## 🔹 6. Traversing an Array

```c
for (int i = 0; i < n; i++) {
    printf("%d ", arr[i]);
}
```

---

## 🔹 7. Common Operations

* **Insertion** → Requires shifting elements → `O(n)`
* **Deletion** → Also requires shifting → `O(n)`
* **Searching**

  * Linear Search → `O(n)`
  * Binary Search (sorted array) → `O(log n)`

---

## 🔹 8. Types of Arrays

1. **1D Array** → Linear list

   ```c
   int arr[10];
   ```
2. **2D Array** → Matrix form

   ```c
   int mat[3][4];
   ```
3. **Multi-Dimensional Arrays** → Arrays of arrays

---

## 🔹 9. Arrays vs Other Data Structures

* **Arrays** → Fast indexed access, fixed size
* **Linked Lists** → Flexible size, slower access
* Arrays are the building blocks for **Stacks, Queues, Hash Tables, etc.**

---

## 🔹 10. Limitations of Arrays

❌ Fixed size (cannot grow/shrink dynamically)
❌ Costly insertions/deletions in the middle
❌ Accessing out-of-bounds index → **Undefined behavior in C**

---

## 🔹 11. Analogy

👉 Think of an **array like mailboxes in a row**.
Each box has a number (index) and stores one item (element).
You can jump directly to a mailbox if you know its number.

---

## 🔹 12. Summary Table

| Concept       | Description                                             |
| ------------- | ------------------------------------------------------- |
| Definition    | Collection of same-type elements in contiguous memory   |
| Access Time   | O(1) random access                                      |
| Memory Layout | Sequential (cache-friendly)                             |
| Operations    | Traversal, insertion, deletion, searching               |
| Types         | 1D, 2D, Multi-Dimensional                               |
| Advantages    | Fast access, efficient, widely used                     |
| Drawbacks     | Fixed size, costly mid-insert/delete, unsafe if misused |

