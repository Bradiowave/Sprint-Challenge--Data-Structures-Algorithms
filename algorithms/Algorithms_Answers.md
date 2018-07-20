Add your answers to the Algorithms exercises here.

### Exercise I.

a) O(n^2) //actaully O(n)

b) O(log n)

c) O(log n) //actually O(sqrt(n))

d) O(n^2)

e) O(n^2) //actaully O(n^3)

f) O(n)

g) O(n)


### Exercise II.

a) 

def find_max_value(a):
    min = a[0]
    max = a[0]

    for num in a:
        if num < min:
            min = num
        if num > max:
            max = num

    return max - min


b) We can follow the pattern of a binary search algorithm to minimize the amount of dropped eggs. 

    Step 1.) We drop an egg from the middle floor and see if it breaks or not. 
    Step 2.) If the egg breaks, we know that all floors above will break the egg, so we must look instead at all of the lower          floors and treat that as our new building. If the egg does not break, we know that all the floors below will not          break the egg, so we look at all of the floors above and treat that as our new building.

    What ends up happening is we discard half of the floors for each test and hone in on the maximum floor that the egg can safely be dropped from.


### Exercise III.

a) The running time would still be O(n) because the quicksort doesn't know that the input array is already sorted. It will still go through each element and put it in the appropriate array, and work on each sub-array recursively until the sub array is of length 1 or less.

b) Even if the pivot was chosen as the median, the running time would still be O(n). If we don't manually change the quicksort algorithm to make use of known information (such as the pivot being the median of the list), then it doesn't matter what pivot point is chosen. It will always iterate through the entire list of numbers.


