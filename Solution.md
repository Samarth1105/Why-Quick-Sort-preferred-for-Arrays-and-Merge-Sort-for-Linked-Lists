# Space optimised Quick Sort for Arrays vs In place merging of LL in Merge Sort

## Quick Sort is preferred for arrays due to several key advantages:
1. In-place Sorting:
  - Quick Sort is an in-place sorting algorithm, meaning it doesn't require any additional memory beyond a small stack for recursion.
  - In contrast, Merge Sort requires additional memory to store temporary arrays during the merging process.
    
2. Cache Efficiency:
  - Arrays have good cache locality, meaning accessing elements sequentially (as is done in Quick Sort) leverages the CPU cache efficiently. Since Quick Sort works by partitioning the array and accessing elements in a sequential manner, it performs well with arrays, leading to faster access times.
  - Merge Sort, on the other hand, can have more scattered memory access due to its use of temporary arrays, which may not benefit as much from cache locality.
    
3. Average-case Time Complexity:
  - Quick Sort's average-case time complexity is O(n log n), which is the same as Merge Sort. However, its constant factors tend to be smaller, making it faster in practice for most inputs.
  - Quick Sort’s worst-case time complexity is O(n²), but this can be mitigated by using techniques like randomized pivot selection, making it perform closer to the average case even in practical scenarios.

## Merge Sort is typically preferred for linked lists due to the way linked lists are structured:
1. Efficient Merging:
  - Merge Sort works very well with linked lists because merging two sorted linked lists can be done in O(1) extra space. This is due to the fact that you can easily rearrange the next pointers of nodes to merge the lists without needing extra memory.
  - In contrast, Quick Sort requires frequent random access to elements (to choose pivots and partition the list), which is inefficient in linked lists since accessing a particular element takes O(n) time due to the sequential nature of linked lists (no direct access).

2. Non-in-place Nature of Merge Sort:
  - Merge Sort is not an in-place algorithm when applied to arrays (because it requires extra space for temporary arrays), but when applied to linked lists, it can be done in-place because the merging process only involves changing next pointers

3. Recursion-Friendly:
  - Since linked lists do not have random access, algorithms that rely on dividing the list (like Merge Sort) are more naturally suited. Merge Sort can recursively divide the list by simply adjusting the next pointers without needing random access, while Quick Sort struggles due to its dependence on partitioning.


