# Why-Quick-Sort-preferred-for-Arrays-and-Merge-Sort-for-Linked-Lists

- Both quicksort and mergesort algorithms are based on the divide and conquer approach. The quick sort is an internal sorting algorithm where the data is sorted in the main memory. In contrast, merge sort is an external sorting algorithm in which the data cannot be stored in the main memory and thus requires an  Auxiliary memory for Sorting the algorithm.

- In quick sort, the arrays are divided into any ratio as there is no compulsion to divide them into equal parts. Whereas in merge sort, the array is divided into two halves only.

- Merge sort is more stable than quick sort, as two elements having equal values appear in the same order in the sorted output as they were in the unsorted input. Quick sort becomes unstable for this scenario. But we can make it stable by making some changes in the code.

- The worst-case complexity of quick sort is O(n^2), as there is a need for many comparisons in the worst condition. In merge sort, worst and average cases have the same complexities O(n*log n).
