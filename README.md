# Bipartite-Matching
Python Code to take bipartite graph, reduce it to max flow graph and finding the maximum Matching for the graph	

**PROBLEM STATEMENT** 

Find the greatest matching between the left and right sides of an undirected bipartite graph. Each node in the left half L linked minimum of one node in the right half R. 

**Interest for the Problem**

We were looking for problems on graphs, and assumed this would be good one since this solution helps in lot of scalability and performance in computing. One real world problem can be a number of job positions and its applicants, matching of multilevel image features in object recognition.

**Goal** 

The Goal of this work is to maximise the number of Matchings. 

**Algorithm**

— Create a directed graph to convert the problem to a Max Flow / Min Cut problem. 

— Make all edges from L to R directed with capacity 1. A flow of 1 corresponds to yes there's a matching and 0 mean no matching.

— Create directed edges from S to every vertex in the left half with capacity 1.

— Create directed edges from every vertex in the right half to T with capacity 1.

— We used  Ford-Fulkerson algorithm / Edmonds karp and breadth For Search, Depth For Search  to find the max flow. 

**Approach for solving the problem**

We take the nodes that has to be mapped as an input argument I.e; left map to right map. 

We add source and target nodes on either sides of the graph and update edge capacities. 

We then build adjacency matrix by adding the edge capacities as one  to the nodes that match left to right else zero. 

We then implement min cut algorithms to get maximum matchings. 

**Worked by**

Abhishek Chintalapati(EC82333)

Sai Sragvi Vibhushan Nidamarti(GT73213)
