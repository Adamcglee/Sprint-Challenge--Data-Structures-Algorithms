Add your answers to the Algorithms exercises here.

```
a)  a = 0  => O(1)
    while (a < n * n * n) => O(N)
      a = a + n * n  => O(1)
```
*O(1) + O(n) + O(1) = [O(n)]*

```
b)  sum = 0 => O(1)
    for (i = 0; i < n; i++) => O(n)
      for (j = i + 1; j < n; j++) => O(n)
        for (k = j + 1; k < n; k++) => O(n)
          for (l = k + 1; l < 10 + k; l++) => O(1) => O(n)
            sum++ => O(1)
```
*O(1) + O(n) + O(n) + O(n) + O(n) + O(1) = [O(n^4)]*

```
c)  bunnyEars = function(bunnies) {
      if (bunnies == 0) return 0 => O(1)
      return 2 + bunnyEars(bunnies-1) => O(n)
    }
```
*O(1) + O(n) = [O(n)]*