# Tic-Tac-Toe
This is a simple, turn-based Tic-Tac-Toe game where the human player ("X") inputs moves, and the computer ("O") chooses random spots. The game detects wins, ties, and invalid moves, and switches players automatically. This code implements a simple Tic-Tac-Toe game in Python, where a human player competes against a computer. Here's a breakdown:

Game Setup:

1. The game board is a list with 9 slots, represented by "-" initially.
2. currentPlayer alternates between "X" (human) and "O" (computer).
3. winner stores the game's winner.
4. gameRunning determines if the game is active.

Functions:

1. printBoard: Displays the board in a grid format.
2. playerInput: Allows the player to select a spot (1-9) to place their marker. It checks for invalid input (if the spot is already taken).
3. Win Check Functions:
   1. checkHorizontle: Checks for a winning row.
   2. checkRow: Checks for a winning column.
   3. checkDiag: Checks for a winning diagonal.
   4. checkIfWin: Calls the above functions to determine a winner, prints the winner, and ends the game.
4. checkIfTie: Ends the game if the board is full and no one has won.
5. switchPlayer: Alternates between "X" and "O".
6. computer: Randomly selects an empty spot on the board for the computer's move.

Game Loop:

1. Continuously runs while gameRunning is True.
2. The board is printed, and the player and computer alternate taking turns.
3. After each move, the game checks for a winner or a tie.
4. The loop ends when the game is won or tied.
