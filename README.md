# ai-tic-tac-toe

Browser-based tic-tac-toe against an AI opponent.

## Play

Open `index.html` in a browser. You play as X, and the AI plays as O. Select an empty square to make a move. Choose **New round** to clear the board while keeping the match score.

## Rules and Gameplay Strategy

### Rules

- The game uses a 3×3 board. X takes the first turn, and players alternate turns placing their mark in an empty cell.
- A player wins by placing three of their marks in a row, column, or diagonal.
- The game is a draw when all cells are filled and neither player has won.
- Once a player wins or the game is drawn, no further moves are made.

### AI Strategy

The AI chooses a legal move using this priority:

1. Complete a line to win immediately.
2. Block the opponent from completing a line on their next turn.
3. Create a fork, or block the opponent from creating one. A fork gives a player two ways to win on a later turn.
4. Take the center if it is available.
5. Take the corner opposite the opponent's mark, then another available corner.
6. Take an available side cell.
