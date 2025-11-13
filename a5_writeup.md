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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them? 

I have learned how to implement DFS and BFS into code when making a program that needs it, even if i still stuggle to understand how to actually implement any of it. I learned about deep and surface copying and when each should be used, and nothing much more. It's not easy to understand anything that is going on. 



2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?
If I ever have to make another game that involves moves and finding the best possible choices for each move like chess, then I could use BFS or DFS. I can't think of much more as I haven't exactly absorbed much from this. 


3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

A LIFO data structure starts from the last thing pushed into the stack, and goes down until it reaches the first thing pushed into the stack. Its the opposite with the FIFO, which starts at the first thing pushed, as it was first in line. LIFO works with DFS as we go as deep as we can without going back to the other things we just checked, while with FIFO, we just go to what ever is next and check it, which works with BFS as we aren't going deep into anything specific. The stack works by putting vales as an actual stack, which is why te last thing pushed into the stack will be the first to be accessed, but a Queue will put everything queued into a line, so the first thing queued will be the first one out. 