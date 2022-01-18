# Sudoku Solver


## Description

The Sudoku Solver takes a [Sudoku puzzle](https://en.wikipedia.org/wiki/Sudoku), and uses backtracking to solve it by checking the empty spaces for which numbers fit. The task is done using several functions. First, it will check for empty slots in the board that is provided in the function (labeled with 0s), and then will take that position in the board and check for which numbers (starting with 1 and ascending to 9) can fit there based on the "valid" function, which checks if that same number is already in the row, column, or box; if the number works, it will be placed in that square. Then it will find the next empty square to see which number works with the same process. If nothing fits, it will backtrack to the previously replaced square and see if another number works so that the previous number can be used elsewhere. The program will do this until all numbers work, or else will return False. Lastly, if the function returns True, it will print out the new, solved board.

## Usage

To use this solver, all you will need is a current version of Python. The function to solve however, requires a Sudoku puzzle in the format of a list of 10 lists with 10 numbers in them. An example is below:

```python
board = [
    [7,8,0,4,0,0,1,2,0],
    [6,0,0,0,7,5,0,0,9],
    [0,0,0,6,0,1,0,7,8],
    [0,0,7,0,4,0,2,6,0],
    [0,0,1,0,5,0,9,3,0],
    [9,0,4,0,6,0,0,0,5],
    [0,7,0,3,0,0,0,1,2],
    [1,2,0,0,0,7,4,0,0],
    [0,4,9,2,0,6,0,0,7]
]
```

## Credits

The Sudoku Solver was created with help from [Tech with Tim](https://www.youtube.com/channel/UC4JX40jDee_tINbkjycV4Sg) on YouTube.
