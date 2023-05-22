## Fortune's algorithm for computing Voronoi diagrams

The initialization of the algorithm, including setting up the data structures and 
inserting the points, takes O(nlog(n)) time, where n is the number of input points.
This is because the points are inserted into a priority queue, which has a time complexity
of **O(log(n))** per insertion, and there are n points.


The main part of the algorithm involves processing the events, both site events and circle events, 
until there are no more events left. Each event processing step involves updating the data 
structures and potentially creating new events.  The overall time complexity of processing 
the events is **O(nlog(n))**, as each event takes **O(log(n))** time to process, 
and there can be up to n events in total.


The algorithm finishes by processing the remaining circle events and performing some final edge calculations.
The processing of the remaining circle events has a time complexity of O(nlog(n)) as well.


Therefore, the overall time complexity of the Voronoi Fortune algorithm 
implemented in this code is **O(nlog(n))**. 
This makes it an efficient implementation for computing Voronoi diagrams.