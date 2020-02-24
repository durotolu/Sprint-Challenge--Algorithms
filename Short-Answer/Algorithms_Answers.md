#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)
O(n)
the while loop iterates until its nth iteration at which point:
a === n ** 3 because a = n(n ** 2)

b)
O(nlogn)
the j *= 2 line constrains the while to less than n times as n gets bigger

c)
O(n)
the function makes n recursive calls with n-1 on every n call
## Exercise II

n = number of floors
middle = n/2
f-1 = threshold floor

find the middle of n and throw the first egg from there
  if it breaks, find the middle of 0th floor to the middle and assign it as the new middle
  if it doesn't break, find the middle of nth floor to the middle and assign it as the new middle
      throw from there and depending on the outcome find middle of current floor and last floor with the opposite outcome
repeat until consecutive floors with opposite outcomes.
f = higher of the 2 consecutive floors

method similar to binary search

runtime = O(logn)