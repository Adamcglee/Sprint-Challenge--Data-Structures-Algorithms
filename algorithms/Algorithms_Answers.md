Add your answers to the Algorithms exercises here.

```
a)  a = 0
    while (a < n * n * n) 
      a = a + n * n
```
```
b)  sum = 0
    for (i = 0; i < n; i++)
      for (j = i + 1; j < n; j++)
        for (k = j + 1; k < n; k++)
          for (l = k + 1; l < 10 + k; l++)
            sum++
```
```
c)  bunnyEars = function(bunnies) {
      if (bunnies == 0) return 0
      return 2 + bunnyEars(bunnies-1)
    }
```