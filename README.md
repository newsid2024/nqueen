# N-Queen Visualiser

![N-Queen-visualisation](visualisation.gif)

The N-Queens puzzle is a classic problem in the field of computer science and mathematics. The objective is to place N chess queens on an N×N chessboard in such a way that no two queens threaten each other. This means that no two queens can share the same row, column, or diagonal.

One way to approach this problem is by using a recursive algorithm. Here's a step-by-step explanation of the algorithm:

Base Case: Start with the first row of the chessboard. For each square in the first row, try placing a queen and move to the next row.

Recursive Step: When placing a queen in a certain row, we need to check if it conflicts with any previously placed queens. To do this, we check the column, upper-left diagonal, and upper-right diagonal from the current position. If there is no conflict, we proceed to the next row and repeat the process.

Backtracking: If at any point we find that we cannot place a queen in a valid position in the current row without conflicts, we backtrack to the previous row and try a different position for the queen in that row. This involves undoing the placement of queens in the subsequent rows and exploring other possibilities.

Solution Found: Continue this process recursively until all N queens are placed on the board without conflicts. When a valid placement of queens is found, it represents a solution to the puzzle.

Explore All Possibilities: The recursive algorithm explores all possible configurations of queen placements, considering different combinations and positions. This back-and-forth exploration is what makes the algorithm a "backtracking" algorithm.

Multiple Solutions: Depending on the initial conditions and the specific N value, there might be multiple valid solutions to the puzzle. The algorithm can be set up to find and list all possible solutions.

Efficiency: While the brute-force recursive algorithm can find solutions for small N values, it becomes computationally expensive as N increases due to the large number of possibilities to explore. Various optimizations and pruning techniques can be applied to make the algorithm more efficient.


