Add your answers to the Algorithms exercises here.

a)  a = 0
    while (a < n * n * n):
      a = a + n * n

    It appears to be an O(n) function

b) sum = 0
    for i in range(n):
      i += 1
      for j in range(i + 1, n):
        j += 1
        for k in range(j + 1, n):
          k += 1
          for l in range(k + 1, 10 + k):
            l += 1
            sum += 1