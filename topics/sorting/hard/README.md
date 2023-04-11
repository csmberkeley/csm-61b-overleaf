# RGB Sort (Radix Go Brrr Sort)
Input: `char[] input;`

You are only allowed to **swap** elements, alter the array such that the array ends up sorted.
For example, given the array ['G', 'B', 'R', 'R', 'B', 'R', 'G'], it should become ['R', 'R', 'R', 'G', 'G', 'B', 'B'].
Your sorting algorithm should take a linear time complexity.

Python pseudocode for a solution:
```py
def rgbSort(x):
    rCount = 0
    gCount = 0
    bCount = len(x) - 1
    while gCount <= bCount:
        if x[gCount] == 'R':
            x[rCount], x[gCount] = x[gCount], x[rCount] 
            rCount += 1
            gCount += 1
        elif x[gCount] == 'G':
            gCount += 1
        elif x[gCount] == 'B':
            x[gCount], x[bCount] = x[bCount], x[gCount]
            bCount -= 1
```
