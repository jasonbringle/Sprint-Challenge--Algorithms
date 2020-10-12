#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)O(c)  No aspect of this function relies on the size of N to run additional times.  No matter how big n is it will aways run at a constant time.


b)O(nlogn)  For each element sized n it will run an additional operation(The while loop).  Log-linear is defined by having to do additional work on something after it iterates


c)O(n)  This recursion runs based on the size of n..  The addition in the return statement when recursing is O(c) so it is not included in the calculation

## Exercise II


N Story Building
if egg thrown off f >= Egg breaks
if egg thrown off f <  Egg unharmed

This sounds like it could be a binary search situation where the middle of the floor numbers is selected and then if the egg is dropped and then breaks then the next floor selected would be the upper half of the array of floors.  We'd split that upper half and drop again. We'd repeat this process even when the egg doesn't break but we would select the lower floors to split... again following the same rules.  By the final number we would know which floor was the highest number floor we could throw and not break from.

The run time complexity of this would be O(logn) because we are not looking at all the elements.
We would sort the array and then cut it in half to search smaller and smaller sections... unlike O(n) where we would look at each item every time we performed an action. And unlike O(n) where we would look at each element and the oeration would increase depending on the size of n.