# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

DFS usually solves Sudoku puzzles faster because it explores one path deeply before backtracking, while BFS explores all options at each step, which can take more time. Use DFS for puzzles with fewer solutions and BFS for more complex situations.

How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

A Stack for DFS allows easy backtracking, while a Queue for BFS helps explore all options at the same level. Other structures like lists or recursion could replace these, but they wouldn’t change the basic idea of DFS or BFS.

Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?


To handle larger puzzles, you can adjust the algorithm to consider more rules and options. The skills learned here, like systematic searching, can help with real-life issues, like planning tasks or managing resources more effectively.