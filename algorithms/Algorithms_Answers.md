Add your answers to the Algorithms exercises here.

**Exercise I**
```
a)  a = 0  
    while (a < n * n * n) 
      a = a + n * n  
```
*[O(n)]*

```
b)  sum = 0 
    for (i = 0; i < n; i++) 
      for (j = i + 1; j < n; j++) 
        for (k = j + 1; k < n; k++) 
          for (l = k + 1; l < 10 + k; l++) 
            sum++ 
```
*[O(n^3)]*

```
c)  bunnyEars = function(bunnies) {
      if (bunnies == 0) return
      return 2 + bunnyEars(bunnies-1) 
    }
```
*O(1) + O(n) = [O(n)]*

**Exercise II**
I would take x = _n_/2 and drop an egg. If it breaks I would take x = (_n_/2)/2 and try it again. If it broke I would divide the floors by 2 again and so on until I reached a floor that the egg would not break. Once I reached a floor that the egg wouldn't break I would move to the floor above that is current_floor + previous(x) / 2 and start moving up. If the egg broke I would split floors back down and so on.