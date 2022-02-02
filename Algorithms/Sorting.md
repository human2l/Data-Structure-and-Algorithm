<img src="Sorting.assets/Screen Shot 2022-02-01 at 3.46.51 PM.png" alt="Screen Shot 2022-02-01 at 3.46.51 PM" style="zoom:50%;" />

# Elementary Sort

### Bubble Sort

swap each two elements if needed to move the largest number to the right

Usage condition: NEVER

### Selection Sort

Human nature sorting way, go through all elements and find the smallest and move to the left

Usage condition: NEVER

### Insertion Sort

1||7,5,3,8,6 => 1,7||5,3,8,6 => 1,5,7||3,8,6 => 1,3,5,7||8,6 => 1,3,5,7,8||6 => 1,3,5,6,7,8

Usage condition: It can be really fast when only a few items and mostly sorted data

# Advanced Sort

### Merge Sort

Divide and Conquer

![Merge-sort-example-300px](Sorting.assets/Merge-sort-example-300px.gif)

Usage condition: Guaranteed fast speed on worst case scenario, however it takes large space O(n), so its better when it alows external sorting which dont care much about space.

### Quick Sort

Divide and Conquer

<img src="Sorting.assets/Screen Shot 2022-02-02 at 11.30.31 AM.png" alt="Screen Shot 2022-02-02 at 11.30.31 AM" style="zoom:50%;" />

Pick a random number as pivot (the last number in the case above), move every smaller elements to the left and larger elements to the right. 

Worst case happens when the pivot picked is the largest/smallest element.

Usage condition: If we dont care about worst case, Quicksort provide fast speed and least space complexity.

### Heapsort

https://brilliant.org/wiki/heap-sort/

Usage condition: Most case slower than Quicksort, using when unless we care both worst case and space usage.

# Stable Sort vs Unstable Sort

### Stable sort:

Merge Sort, Timsort, Counting Sort, Insertion Sort, Bubble Sort

### Unstable sort:

Others such as Quicksort, Heapsort and Selection Sort

<img src="Sorting.assets/Screen Shot 2022-02-02 at 10.48.09 AM.png" alt="Screen Shot 2022-02-02 at 10.48.09 AM" style="zoom:50%;" />

# Can we beat nlog(n)?

<img src="Sorting.assets/Screen Shot 2022-02-02 at 12.02.49 PM.png" alt="Screen Shot 2022-02-02 at 12.02.49 PM" style="zoom:50%;" />

Counting Sort and Radix Sort only work on NUMBERS or fixed length integers

# Resources

Sorting animation: https://www.toptal.com/developers/sorting-algorithms

Quicksort vs heapsort:https://stackoverflow.com/questions/2467751/quicksort-vs-heapsort

## Radix Sort + Counting Sort

Radix Sort: https://brilliant.org/wiki/radix-sort/

Radix Sort Animation: https://www.cs.usfca.edu/~galles/visualization/RadixSort.html

Counting Sort: https://brilliant.org/wiki/counting-sort/

Counting Sort Animation: https://www.cs.usfca.edu/~galles/visualization/CountingSort.html