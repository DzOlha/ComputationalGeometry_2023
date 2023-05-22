
## Bentley-Ottmann Sweep Line algorithm
The time complexity of the Bentley-Ottmann algorithm implemented in this lab work is **O((n + k) log n)**, 
where n is the number of line segments and k is the number of intersections. 


This complexity arises from sorting the end points of the line segments, 
which takes O((n + k) log n) time using an efficient sorting algorithm.


The sweep line algorithm itself performs various operations such as 
insertion and deletion in the binary search tree, which takes O(log n) time in the average case.
However, in the worst case, where there are many intersections, the complexity can reach O((n + k) log n).


The space complexity of the algorithm is **O(n)**, as it stores the line segments and the binary search tree.