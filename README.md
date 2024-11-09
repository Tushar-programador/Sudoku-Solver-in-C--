# Sudoku Solver with Enhanced Features

This project is a Sudoku Solver implemented in C++ using the backtracking algorithm. It solves a given Sudoku puzzle and offers additional features like generating puzzles, tracking recursion calls, and showing the total time taken to solve the puzzle. It also includes a simple Sudoku puzzle generator for creating random puzzles with varying difficulty.

## Features

- **Sudoku Solver**: Solves a given Sudoku puzzle using the backtracking algorithm.
- **Puzzle Generator**: Generates a random Sudoku puzzle with a specified number of pre-filled cells.
- **Recursion Count**: Tracks the number of recursive calls the backtracking algorithm makes to solve the puzzle.
- **Puzzle Display**: Displays the Sudoku puzzle at each stage (initial, solved, and generated).
- **Easy Difficulty Level**: Generates a puzzle with a user-specified number of pre-filled cells.

## Requirements

- C++ compiler (e.g., **g++** or **clang++**)
- Basic understanding of the Sudoku game and backtracking algorithm

## Installation

To get started with the Sudoku Solver, follow these steps:

1. **Clone the repository** (or copy the code into a file):
   ```bash
   git clone https://github.com/Tushar-programador/sudoku-solver.git
   
2. **Navigate to the project directory**:
   ```bash
    cd sudoku-solver
3. **Compile the program**:
   ```bash
   g++ -o sudoku_solver sudoku_solver.cpp

## Usage
The program will first display an initial Sudoku puzzle.
It will then solve the puzzle and display the solved grid.
Finally, it will display the generated Sudoku puzzle with a specified number of pre-filled cells.
The program will also show the total number of recursion calls the backtracking algorithm makes to solve the puzzle.


## Example Output:

```output
Initial Sudoku Puzzle:
5 3 0 0 7 0 0 0 0 
6 0 0 1 9 5 0 0 0 
0 9 8 0 0 0 0 6 0 
8 0 0 0 6 0 0 0 3 
4 0 0 8 0 3 0 0 1 
7 0 0 0 2 0 0 0 6 
0 6 0 0 0 0 2 8 0 
0 0 0 4 1 9 0 0 5 
0 0 0 0 8 0 0 7 9 

Solved Sudoku Puzzle:
5 3 4 6 7 8 9 1 2 
6 7 2 1 9 5 3 4 8 
1 9 8 3 4 2 5 6 7 
8 5 9 7 6 1 4 2 3 
4 2 6 8 5 3 7 9 1 
7 1 3 9 2 4 8 5 6 
9 6 1 5 3 7 2 8 4 
2 8 7 4 1 9 6 3 5 
3 4 5 2 8 6 1 7 9 

Total Recursion Calls: 107

Generated Sudoku Puzzle:
0 0 0 0 7 0 0 0 0 
0 0 0 1 9 0 0 0 5 
0 0 0 0 0 5 0 0 0 
0 0 0 0 6 0 0 8 0 
4 0 0 0 0 3 0 0 0 
7 0 0 0 2 0 0 0 0 
0 0 3 0 0 0 2 8 0 
0 0 5 4 1 9 0 0 0 
0 0 0 0 8 0 0 7 9
```
## Customizing the Puzzle Generator
You can adjust the number of pre-filled cells in the generated puzzle by modifying the generatePuzzle function's argument:
```cpp
generatePuzzle(newGrid, 30);  // Change 30 to any number between 0 and 81 for difficulty
```
Low numbers (e.g., 30): Easier puzzle (more cells filled).
Higher numbers (e.g., 50-60): Harder puzzle (fewer cells filled).

## Acknowledgements
Thanks to all those who contributed to the development of the backtracking algorithm and Sudoku game mechanics.
Inspired by various C++ algorithms and data structures available on platforms like GeeksforGeeks.
