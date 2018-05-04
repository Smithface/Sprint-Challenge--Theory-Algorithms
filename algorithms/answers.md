# Exercise I.
Give an analysis of the running time with respect to the input size n of each of the following program fragments below:
```
a)

a = 0;
while (a < n * n * n) {   // O(n^3)
  a = a + n * n;
}
```
## O(n^3^)

---
```
b) // input array is of length n

i = array.length - 1;
while (array[i] > x && i >= 0) {
  i = i/2;
}
```
## O(log~2~(n))

```
c)

sum = 0;
for (i = 0; i < Math.sqrt(n) / 2; i++) {    //sqrt(n)/2
  for ( j = i; j < 8 + i; j++) {            //constant
    for (k = j; k < 8 + j; k++) {           //constant
      sum++;
    }
  }
}
```
## O(1/2 * sqrt(n)) -> O(sqrt(n))

```
d)

sum = 0;
for (i = 1; i < n; i *= 2) {      //log(n)
  for (j = 0; j < n; j++) {       //n
    sum++;
  }
}
```
## O(n log~2~(n))

```
e)

sum = 0;
for (i = 0; i < n; i++) {                  //n
  for (j = i + 1; j < n; j++) {            //n
    for (k = j + 1; k < n; k++) {          //n
      for (l = k + 1; l < 10 + k; l++) {   //constant
        sum++;
      }
    }
  }
}
```
## O (n^3^)

```
f)

bunnyEars = function (bunnies) { // here bunnies === n
  if (bunnies === 0) return 0;
  return 2 + bunnyEars(bunnies-1);          //will be called n times
}
```
## O(n)

```
g)

search = function (array, arraySize, target) { // here arraySize === n
  if (arraySize > 0) {
    if (array[arraySize-1] === target) return true;
  } else {
    return search(array, arraySize-1, target);
  } 
  return false;
}
```
## O(n)
