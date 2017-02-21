# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Once naked twins are identified in a given unit, this adds a constraint to other boxes in the same unit: none of them can have any of the naked twins digits as both can only be in one of the naked twins boxes. Hence, this constraint can be applied to all other boxes in the unit, therefore reducing possibilites. 

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Original sudoku rules impose some contraints: all numbers from 1 to 9 must be in all rows, all columns and all 3x3 squares. Diagonal sudoku only imposes a new contraint: diagonals must have all numbers from 1 to 9 as well. Current provided algorithms already take care of handling all constraints imposed through list 'unitlist'. Adding diagonals to 'unitlist' will imposed the desired constraints.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.