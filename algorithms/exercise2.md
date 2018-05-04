# Exercise II.
```
a)
Given an array a of n numbers, design a linear running time algorithm to ﬁnd the maximum value of a[j] - a[i], where j ≥ i.

let max, min;
for(let i = 0; i < n; i++) {
  max = Math.max(arr[i], max);
  min = Math.min(arr[i], min);
}

return max - min;
```

```
b)
Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg is broken if it is thrown oﬀ ﬂoor f or higher, and unbroken otherwise. Devise a strategy to determine the value of f such that the number of dropped eggs is minimized.

If we use the devide and conquer approach, we can minimize the number of dropped eggs to O(log<sub>2</sub>(n)).
```
