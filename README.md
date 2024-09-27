# Insertion_sort
Patika.dev Data Science course example

## Insertion Sort Algorithm

Insertion Sort works by dividing the list into two parts: the sorted part and the unsorted part. It repeatedly takes the next element from the unsorted part and inserts it into the correct position in the sorted part.

### Steps:
1. Start with the first element, considering it as sorted.
2. Take the next element and compare it with elements in the sorted part.
3. Shift all elements greater than the current element to the right.
4. Insert the current element into its correct position.
5. Repeat the process for all elements.

### Time Complexity:
- Best case: O(n) when the array is already sorted. We have to check all elements in the array. There are 'n' elements, so we perform 'n' checks. This means that there are n process.
- Worst case: O(n^2) when the array is sorted in reverse order. We compare n elements with other n elements. Since we compare n elements n times, the worst-case is n^2.

### Example:
[22,27,16,2,18,6] 
We apply insertion-sort to this array. We will compare all elements with each other in order. 
- [22,27,16,2,18,6] Compare 27 with 22. There is no problem. Keep going.
- [16,22,27,2,18,6] Compare 16 with 22 and 27. Move 16 to the zero index of the array.
- [2,16,22,27,18,6] Compare 2 with 16, 22 and 27. Move 2 to the zero index of the array.
- [2,16,18,22,27,6] Compare 18 with 2, 16, 22 and 27. Move 18 to the second index of the array.
- [2,6,16,18,22,27] Compare 6 with 2, 16, 18, 22, and 27. Move 6 to the first index of the array.

### Big-O Notation: 
Firstly, we compare the second element with the first element. So we do one process. When we compare other elements with previous elements, each time the number of processes increases by 1. 
1+2+3+.......+(n-1)+n=(n*(n+1))/2 => n^2/2 As a result Big-O is O(n^2).
  
If we try to find 18 in the array, we can find it in the average case due to the position in the array. 
