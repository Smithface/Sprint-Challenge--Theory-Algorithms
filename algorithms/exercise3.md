Exercise III. Below is the the pseudo-code for the Quicksort algorithm:

```
function quicksort(array)
  if length(array) <= 1
    return array
  select and remove a pivot element pivot from array
  create empty lists less and greater
  for each x in array
    if x <= pivot then append x to less
    else append x to greater
  return concatenate(quicksort(less), list(pivot), quicksort(greater))
```
a) Suppose we implement quicksort so that the pivot is always chosen to be the ﬁrst element of the array. What is the running time of this algorithm on an input array that is already sorted? Why?

* At best (no repeating elements), the running time is O(n). At worst, the running time is O(n<sup>2</sup>).

b) Suppose we implement quicksort so that the pivot is always magically chosen to be the median element of the array. What is the running time of this algorithm? Why?

* The running time of this algorithm would be O(log<sub>2</sub>(n)) because it would become a divide and conquer approach. (the internet says the best is O(n log(n)), so I'm not sure about this one.)
