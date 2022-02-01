# Sudoku Solver

The Sudoku Solver takes a [Sudoku puzzle](https://en.wikipedia.org/wiki/Sudoku), and uses backtracking with Python to solve it by checking the empty spaces for which numbers fit.

## Description

The Sudoku Solver uses several functions to complete the puzzle. First, it will check for empty spot (labeled with 0s) in the board using the "find_empty" function. Then, it will take that position in the board (based on column and row) and check for which numbers (starting with 1 and ascending to 9) can fit there using the "valid" function, which checks if that same number is already in the row, column, or box; if the number works, it will be placed in that spot. Then it will find the next empty spot to see which number works with the same process. If nothing fits, it will backtrack to the previously replaced spoit and see if another number works so that the previous number can be used elsewhere. The program will do this until all numbers work, or else will return False. Lastly, if the function returns True, it will print out the new, solved board.

## Usage

To use this solver, all you will need is a current version of Python. The function to solve however, requires a Sudoku puzzle/board in the format of a list of 9 lists with 9 numbers in them. An example is below:

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
Then, run the file and watch Python print a solved board!

## Credits

The Sudoku Solver was created with help from [Tech with Tim](https://www.youtube.com/channel/UC4JX40jDee_tINbkjycV4Sg) on YouTube.
