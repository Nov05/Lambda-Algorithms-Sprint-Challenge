#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  a = 0
    while (a < n * n * n):
      a = a + n * n

O(n)


b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1

O(n * log2 n)


c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)

O(n)

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

Answer: binary search

1. drop an egg off floor n/2: if broken, try n/2/2; if not, try n/2 + (n-n/2).
2. repeat the steps until there is only one number left and it cannot break into smaller intervals.


