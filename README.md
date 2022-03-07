# Data-Structure---Bubble-Sort-Algorithm
Bubble sort is a simple sorting algorithm. This sorting algorithm is comparison-based algorithm in which each pair of adjacent elements is compared and the elements are swapped if they are not in order. This algorithm is not suitable for large data sets as its average and worst case complexity are of Ο(n2) where n is the number of items.
## How Bubble Sort Works?
We take an unsorted array for our example. Bubble sort takes Ο(n2) time, so we're keeping it short and precise.

![](./assests%20/Picture1.png)

Bubble sort starts with very first two elements, comparing them to check which one is greater.

![](./assests%20/picture2.png)

In this case, value 33 is greater than 14, so it is already in sorted locations. Next, we compare 33 with 27.

![](./assests%20/picture3.png)

We find that 27 is smaller than 33 and these two values must be swapped.

![](./assests%20/picture4.png)

The new array should look like this −

![](./assests%20/picture5.png)

Next we compare 33 and 35. We find that both are in already sorted positions.

![](./assests%20/picture6.png)

Then we move to the next two values, 35 and 10.

![](./assests%20/picture7.png)

We know then that 10 is smaller 35. Hence they are not sorted.

![](./assests%20/picture8.png)

We swap these values. We find that we have reached the end of the array. After one iteration, the array should look like this −

![](./assests%20/picture9.png)

To be precise, we are now showing how an array should look like after each iteration. After the second iteration, it should look like this −

![](./assests%20/picture10.png)

Notice that after each iteration, at least one value moves at the end.

![](./assests%20/picture11.png)

And when there's no swap required, bubble sorts learns that an array is completely sorted.

![](./assests%20/picture12.png)

Now we should look into some practical aspects of bubble sort.

## Algorithm

We assume list is an array of n elements. We further assume that swap function swaps the values of the given array elements.

![](./assests%20/picture13.png)

## Pseudocode
We observe in algorithm that Bubble Sort compares each pair of array element unless the whole array is completely sorted in an ascending order. This may cause a few complexity issues like what if the array needs no more swapping as all the elements are already ascending.

To ease-out the issue, we use one flag variable swapped which will help us see if any swap has happened or not. If no swap has occurred, i.e. the array requires no more processing to be sorted, it will come out of the loop.

Pseudocode of BubbleSort algorithm can be written as follows −

![](./assests%20/picture14.png)

## Implementation

One more issue we did not address in our original algorithm and its improvised pseudocode, is that, after every iteration the highest values settles down at the end of the array. Hence, the next iteration need not include already sorted elements. For this purpose, in our implementation, we restrict the inner loop to avoid already sorted values.




