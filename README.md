<h1 align="center">Big O</h1> <br>
<h2 align="center">computational complexity -  analyzing how long something takes to run</h2> <br>

<p align="center">
Big O is the way we analyze how efficient algorithms are 
</p>

Hence this is what Big O does; we ignore the little parts and concentrate on the big parts. Keeping with 3x² + x + 1, the Big O for this equation would be O(n²) where O is just absorbing all the other fluff (including the factor on the biggest term.)


If we have no loops and just do something and exit/return, then it's said we're doing it in constant time, or O(1).

<img src='https://btholt.github.io/complete-intro-to-computer-science/static/26b7a304a42506939d5959f101b26eb4/5a190/graph-log.png' />

Here we see a graph that represents the more items we put in a array, how long does it take for the function to complete.

constant - The red graph represnts O(1) 

The blue line represents a function that takes longer based on how many items are in the array O(n)

The green line is where we get start getting scary. For every item we add to the array, it takes exponentially more time to complete the operation. Adding 10x the items could cause a function to takes 100x longer since it's O(n²).

The purple line - O(log n) - recursion

<h2 align="center">Spatial  complexity - how much space (e.g. how much RAM or disk space) an algorithm needs to complete.</h2> <br>

### Bubble Sort

The bubble sort is a typical first one to do because it matches the human mental model of sorting pretty well. The algorithm is pretty simple: compare two items in an array that are next to each other. If they're out of order (that is, the larger one comes first in the array) swap them. Then move forward one index, compare again, swap if needed, and continue to the next item in the array. Once we've reached the end of the array, if we've swapped anything in the previous run through, the array could still be out of order, so we have to pass through again. Once we run through the whole array with no swaps, the array is sorted!