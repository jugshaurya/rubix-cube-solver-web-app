# Rubix Cube Solver

-   Can do with DFS/BFS, but no of states in graph are too much to even store a visited array / dp array.

-   Class to implement

    -   All the 18 different rotations of the cube: F, Fprime, F2, U, Uprime, etc.
    -   Print function: A function that takes the Rubik’s Cube and prints it in the Planar Representation Format.
    -   Random Shuffle: A function that returns a randomly shuffled Rubik’s Cube which is solvable.
    -   isSolved(): a boolean function that tells whether the current configuration of the Rubik’s Cube is solved or not.

-   cube[SIDE][ROW][COL] = cube[ i ][ j ][ k ] → color of the ith side, jth row and kth col.

SIDE Mapping
Up → 0 (White)
Left → 1 (Green)
Front → 2 (Red)
Right → 3 (Blue)
Back → 4 (Orange)
Down → 5 (Yellow)

## Note:

-   Not all permutations are solvable

-   There are 43,252,003,274,489,856,000 possible states of Rubik’s Cube. Despite that, in 2010 it was shown that any Rubik’s Cube configuration can be solved in 20 moves or fewer.
    -   Depth-First Search (DFS) + max depth as a Hyper-parameter
    -   Breadth-First Search (BFS)
    -   Iterative-Deepening Depth-First Search (IDDFS)
    -   IDA\* solver using Korf’s Algorithm( combines the A\* algorithm with IDDFS and uses pattern databases as a heuristic.)
