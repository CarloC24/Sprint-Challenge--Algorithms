Add your answers to the Algorithms exercises here.

```
a)  a = 0
    while (a < n * n * n)
      a = a + n * n
```

Space Complexity = 0(1)
---- Since it is only taking 1 space on the memory when the function is ran it has a big 0 of 0(1)

Time Compexity = 0(n)
---- Since when 3 is n the while loop runs three times when 4 is n the loop runs four times so it has a linear number of run time

```
b)  sum = 0
    for i in range(n): # 0(n)
      i += 1
      for j in range(i + 1, n): # n + 1
        j += 1
        for k in range(j + 1, n): # n + 1
          k += 1
          for l in range(k + 1, 10 + k):  0(10) ==> 0(1)
            l += 1
            sum += 1
```

Space Complexity = O(1)
---- 0(1) is the Space Complexity because we are only storing sum in memory and it is explicitly defined

Time Complexity = 0(n(n - 1)^2)
0(n) _ 0(n - 1) _ 0(n - 1) \* 0(1) is the computation so the Big O is 0(n(n - 1)^2)

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```

Space Complexity = 0(1)
---- The function returns the number of bunny ears so the function only uses 1 space in the memory

Time Complexity = 0(n)
---- The function runs on the loop with the number of bunnies we put on the function so it runs 0(n) with n as the number of bunnies
