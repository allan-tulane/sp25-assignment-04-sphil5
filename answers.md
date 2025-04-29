# CMPS 2200 Assignment 5
## Answers

**Name:** Shania Phillips 






- **1a.** log_d(n)


- **1b.** The work for delete-min = O(lg N). The work for insert is O(lg N).
  

- **1c.** O(V log V + E log V)
  

- **1d.** d = V^epsilon


- **2a.** APSP(i,j,k) = min(APSP(i,j,k-1), APSP(i,k,k-1) + APSP(k,j,k-1))


- **2b.** Yes, I do see a relationship between APSP(i, j, 1) and APSP(i, j, 2). APSP(i, j, 2) is the minimum of APSP(i, j, 1) and APSP(i, 2, 1) + APSP(2, j, 1).


- **2c.** APSP(i,j,k) is the minimum of APSP(i,j,k-1) and APSP(i,k,k-1) + APSP(k,j,k-1) is the optimal substructure property for APSP(i,j,k).

- **2d.** Only one subproblem will be computed from scratch. The resulting work of this dynamic programming algorithm is O(n^3).

- **2e.** The work of this algorithm is O(n^3). The work of Johnson's algorithm is O(n^2 log n + (n * E)). Our dynamic programming algorithm is preferable when the number of edges in our graph is close to n^2.



- **3a.** A solution to MST is not guaranteed to be a solution to NMET because MST minimizes the total weight of the edges while NMET minimizes the maximum weighted edge. Therefore a solution that is optimal for MST may not be optimal for NMET and vice versa. 


- **3b.**
  next_best_tree(graph):
    - sort the weight of the edges in nondecreasing order
    - initialize an empty set for the tree
    - for each edge:
      - add the edge to the tree
      - if a spanning tree is formed, return the tree as the next best tree 
  


- **3c.** W = O(E log E) or O(E log V)
