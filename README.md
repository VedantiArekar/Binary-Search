# Binary-Search

A Binary Search is a sorting algorithm, that is used to search an element in a sorted array. A binary search technique works only on a sorted array, so an array must be sorted to apply binary search on the array. It is a searching technique that is better then the liner search technique as the number of iterations decreases in the binary search.

The logic behind the binary search is that there is a key. This key holds the value to be searched. The highest and the lowest value are added and divided by 2. Highest and lowest and the first and last element in the array. The mid value is then compared with the key. If mid is equal to the key, then we get the output directly. Else if the key is greater then mid then the mid+1 becomes the lowest value and the process is repeated on the shortened array. Else if the key value is less then mid, mid-1 becomes the highest value and the process is repeated on the shortened array. If it is not found anywhere, an error message is displayed.

Conditions for when to apply Binary Search in a Data Structure:

To apply binary search in any data structure, the data structure must maintain the following properties:

1. The data structure must be sorted.

2. Access to any element of the data structure takes constant time.

When to use Binary Search?

1. When searching a large dataset as it has a time complexity of O(log n), which means that it is much faster than linear search.

2. When the dataset is sorted.

3. When data is stored in contiguous memory.

4. Data does not have a complex structure or relationships.

How to Implement Binary Search?

The basic steps to perform Binary Search are:

1. Set the low index to the first element of the array and the high index to the last element.

2. Set the middle index to the average of the low and high indices.

   a. If the element at the middle index is the target element, return the middle index.
   
   b. Otherwise, based on the value of the key to be found and the value of the middle element, decide the next search space.
   
      i. If the target is less than the element at the middle index, set the high index to middle index – 1.
      
      ii. If the target is greater than the element at the middle index, set the low index to middle index + 1.
     
3. Perform step 2 repeatedly until the target element is found or the search space is exhausted.
