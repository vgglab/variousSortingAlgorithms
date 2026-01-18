# variousSortingAlgorithms
# 🧠 Sorting Algorithms in Python

## 📌 What I did today

Today I implemented and tested multiple **sorting algorithms from scratch in Python** to understand:

- How sorting algorithms work internally
- Their real execution time
- Practical difference between **O(n²)** and **O(n log n)** algorithms

---

## ✅ Implemented Algorithms

- 🫧 Bubble Sort  
- 🔍 Selection Sort  
- 🔀 Merge Sort (using recursion)  
- 🐒 Monkey Sort (for learning purpose)  
- ⏱️ Sleep Sort (experimental)

All algorithms were implemented using **Object-Oriented Programming (OOP)**.

---

## 🧠 Key Learnings

### 🔁 Recursion
- Learned how merge sort uses **divide and conquer**
- Understood that time calculation must be done **outside recursive calls**
- Used a wrapper function to measure total execution time

---

### ⏱️ Time Measurement
- Used `time.time()` and `time.perf_counter()`
- Learned why `perf_counter()` is more accurate for benchmarking
- Built a fair comparison system for all sorting algorithms

---

## 📊 Time Complexity Comparison

| Algorithm | Best | Average | Worst |
|--------|--------|--------|--------|
| Bubble Sort | O(n) | O(n²) | O(n²) |
| Selection Sort | O(n²) | O(n²) | O(n²) |
| Merge Sort | O(n log n) | O(n log n) | O(n log n) |
| Monkey Sort | — | ∞ | ∞ |
| Sleep Sort | — | Depends on values | — |

---

## ⚡ Performance Result

After testing with large random arrays:

- Bubble Sort → Slow  
- Selection Sort → Slow  
- Merge Sort → ⚡ **Fastest**  
- Monkey Sort → Not practical  
- Sleep Sort → Experimental  

✅ **Merge Sort performed significantly faster than others.**

---

## 🧪 Example Usage

```python
import random
from sorting_algorithms import SortingAlgorithms

arr = random.sample(range(1, 3000), 2000)

s = SortingAlgorithms(arr)
s.mergeSort()
