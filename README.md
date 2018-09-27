# SudokuSolver
A Python console application to solve the standard 9 by 9 Sudoku puzzle.

<b>Input</b><br>
The input Sudoku board is written as a 9x9 grid of integars in range [0,9].<br>
Rows are separated by a newline character (\n).<br>
<b>0 represents an empty square.</b><br>
Examples:
<pre>
240000009
090031000
001590080
000000076
000803000
960000000
030045100
000620090
600000052
</pre>
<pre>
764000100
000070806
809604030
000800063
090351020
580006000
050902301
902010000
006000289
</pre>

<b>Mechanism</b><br>
Solves via recursion.<br>
Upon attempting to solve a Sudoku board:
<ul>
  <li>Check if the board is already solved (base case of recursion)</li>
  <li>Find the different possibilities of each empty square</li>
  <li>Try substituting the square with the least possiblilies with each of its possibilities and solving the newly subsituted board</li>
</ul>
  
<i>Note: Python 3.7+ required for running the .py version.</i>
