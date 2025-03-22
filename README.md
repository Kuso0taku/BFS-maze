# BFS & DFS algorithms

## What's the project about?

 - Find the way out from maze
 - Practice & understand algorithms

## Difference between BFS & DFS

 - **BFS** (Breadth-First Search) explores all neighbors at the present depth before moving to nodes at the next depth level
 - **DFS** (Depth-First Search) explores as far as possible along each branch before backtracking.

## What's the maze?

I wil assume that the maze is a matrix MxN (M rows & N colums).
In program is a *vector* of *bytes* (data type), where:
 - 0 is empty space hwhere I can move
 - 1 is wall I can't get through
 - 2 is me 
 - 83 is start ('cuz 'S' in ASCII is 83)
 - 69 is end ('cuz 'E' in ASCII is 69)
also, we can use 'S' & 'E' instead of 83 & 69.

#### For Example:

**C++**:
> vector<vector<byte>> maze = {
> {83, 1, 0, 0, 1},
> {0, 1, 0, 0, 69},
> {0, 0, 0, 1, 1}
> }

**Golang**:
> maze := [][]byte {
> {83, 1, 0, 0, 1},
> {0, 1, 0, 0, 69},
> {0, 0, 0, 1, 1}
>
