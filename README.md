# Community-Structure-in-Graphs
The aim of this project is to test an algorithm related to recognizing the community structures of Graphs
In the algorithm, by eliminating edges connecting the communities, The whole graph is divided into denser subgraphs.
formulate for giving a score to the graph's edges:
Cij = [Zij + 1] / [Min(Kj-1, Ki-1)]
in which Zij is cycles of length 3 through vertices i and j, 
Ki and Kj are the degrees of vertices i and j, respectively.
The algorithm:
1. Calculating Cij for all edges
2. Sorting edges based on calculated scores
3. Eliminating the edge with minimum Cij
4. Finish if the graph is separated into two parts.
5. Recalculating Cij for edges that are modified after step 3
6. Back to step 1

