# Tic-Tac-Toe with Minimax Algorithm

This project implements a graphical Tic-Tac-Toe game with an AI opponent using the minimax algorithm. The game allows a user to play against the computer, which makes optimal moves to challenge the player.

---

## **Technologies Used**

- **Python**: Core programming language.
- **Pygame**: Used for creating the graphical user interface (GUI).
- **Minimax Algorithm**: Implements decision-making logic for the AI.

---

## **Project Files**

### **`runner.py`**
This file handles:
- The game's graphical interface using Pygame.
- User input and game flow.
- Displaying the game board and status messages.

#### Key Features:
1. **Player Selection**: Choose to play as `X` or `O`.
2. **Interactive Board**: 
   - Displays moves made by the player and AI.
   - Highlights available moves.
3. **Game Status**:
   - Indicates whose turn it is.
   - Displays the winner or declares a tie.
4. **AI Turn**:
   - Uses the minimax algorithm to determine optimal moves.
5. **Play Again Option**: Allows replaying after the game ends.

---

### **`tictactoe.py`**
This file contains the logic for:
- Board state management.
- Validating moves and updating the game board.
- Implementing the minimax algorithm for AI decisions.

#### Key Functions:
1. **`initial_state()`**: Creates an empty 3x3 board.
2. **`player(board)`**: Determines whose turn it is (X or O).
3. **`actions(board)`**: Returns available moves on the board.
4. **`result(board, action)`**: Returns the updated board after a move.
5. **`winner(board)`**: Checks if a player has won.
6. **`terminal(board)`**: Determines if the game is over.
7. **`utility(board)`**: Assigns a score based on the game's outcome:
   - `1`: X wins
   - `-1`: O wins
   - `0`: Tie
8. **`minimax(board)`**: Implements the minimax algorithm to find the optimal move for the AI.

#### Minimax Helper Functions:
- **`max_value(board)`**: Determines the best move for `X`.
- **`min_value(board)`**: Determines the best move for `O`.

---

## **How to Run the Game**

1. **Install Dependencies**:
   Ensure you have Python and Pygame installed:
   ```bash
   pip install pygame
2. **Run the Game: Execute the runner.py file**:

   ```bash
   python runner.py

--- 
**Gameplay**:

Choose to play as X or O.
Click on the board to make your move.
Compete against the AI until the game ends.

---
**How the AI Works**
The AI uses the minimax algorithm to evaluate all possible moves and their outcomes:

Maximizing Player (X): Tries to maximize the score.
Minimizing Player (O): Tries to minimize the score.
Optimal Strategy: The AI chooses the move that guarantees the best possible outcome, assuming the opponent also plays optimally.

---
**Future Improvements**
I've made this game as part of a learning project. Feel free to add any additional features that you find suitable like adding sound effects and animations for moves. Including difficulty levels by adjusting the depth of the minimax algorithm. adding a two-player mode etc.
