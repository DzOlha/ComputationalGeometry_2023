
## Range searching with Range Tree

The lab work implements a range searching algorithm using 
a combination of threaded binary trees and region search trees.
The time complexity of this algorithm is influenced by the 
construction of the trees and the search process.


The construction of the threaded binary tree (build_tb_tree) 
has a time complexity of **O(nlog(n))**, where n is the number of points.
This is because the tree is constructed recursively by dividing the 
points in half at each step, resulting in a balanced tree.


The construction of the region search tree (build_region_tree) also has a time 
complexity of O(nlog(n)), as it recursively divides the interval points to build the tree.


The search process (region_search and y_search) has a time complexity of **O(k + log(n))** 
in the worst case, where k is the number of points within the specified region and n is the total number of points.
. This is because the algorithm traverses the region search tree based on the x region and 
performs a threaded binary tree search based on the y region.


Overall, the algorithm achieves a time complexity of **O(nlog(n))** for 
construction and **O(k + log(n))** for the search process.
This makes it a good implementation of range searching with range trees, 
as it provides efficient search capabilities for finding points within specified regions.
