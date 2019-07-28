_For each of bubble, insertion, and selection 
sort, what are the best and worse case scenarios?_

__Bubble Sort__

Best Case: O(N)

Based on the code in the reading, if the elements are already sorted you still iterate through the entire array comparing each element to every other element up to the last sorted index. This is O(N^2). If you store a variable indicating that no items are swapped on the first pass then you can avoid subsequent checks and achieve O(N) performance.


Worst Case: O(N^2)

If the elements are in reverse order and all unique, you will have to perform the comparison described above.

__Insertion Sort__

Best Case: O(N)

If the elements are already sorted, we still check each element but since they are already in their correct position, comparisons to the first previous element will result in no swaps.

Worst Case: O(N^2)

If the elements are in reverse order, each iteration will require comparing the current element to every element before it and shifting the entire array.

__Selection Sort__
          
Best Case: O(N^2)

If the elements are already sorted you still iterate through the entire array, comparing each element to the element with the minimum value in the current range (which itself requires iterating through the entire range to find that minimum value).

Worst Case: O(N^2)

A distinguishing factor of selection sort is that it's best & worst case scenario are exactly the same because it performs the exact same # of comparisons regardless of the data in the array (ex. if it already sorted).

_Why is the sorting problem a good candidate for divide and conquer?_