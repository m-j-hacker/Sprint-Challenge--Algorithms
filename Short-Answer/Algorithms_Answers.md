Add your answers to the Algorithms exercises here.

a)  a = 0
    while (a < n * n * n):
      a = a + n * n

    It appears to be an O(n) function - the loop condition is n^3
    and it increases by at least n^2 each iteration, which would make that a constant that we can drop to leave us with O(n).

b) sum = 0
    for i in range(n): // n
      i += 1
      for j in range(i + 1, n): // n*n
        j += 1
        for k in range(j + 1, n): // n*n
          k += 1
          for l in range(k + 1, 10 + k): // n*n
            l += 1
            sum += 1

    I think it comes out to being O(n^2) 

c) O(n)

Exercise II

We are dealing with variables n and f, where n is the
number of stories in the building and f is the floor which is the point where eggs dropped will break. 

Our function will take these variables and run an if statement to determine if the inputs are valid (n cannot be lower than f!).
Then, we return which floors are lower than f, and print out
the result - ex. "The floors to be on to prevent broken eggs are 1, 2, and 3" if f is 4 and n is greater than or equal to f