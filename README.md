# Chess-Board-Game-Using-CPP

# Chess Validator

## Problem Statement
Chess is a two-player strategy game played on an 8x8 checkered board. The game starts with a standard board setup and follows specific rules governing piece movements and player turns.

## Rules of the Game
- The game is played between two players, one controlling the white pieces and the other controlling the black pieces.
- Each player has 16 pieces: 1 King, 1 Queen, 2 Knights, 2 Rooks, 2 Bishops, and 8 Pawns.
- Each piece has its own movement rules.
- Players take turns moving their pieces.
- A move can only be made if it follows the piece's movement rules and does not jump over other pieces (except for knights).
- A player may capture an opponent's piece by landing on its position.
- The player controlling the white pieces always moves first.

## Piece Moves
### Pawn
- Moves one step forward.
- Can move two steps forward on its first move if both cells are unoccupied.
- Captures diagonally one step forward.

### Knight
- Moves in an 'L' shape (two steps in one direction and one step perpendicular).
- Can jump over other pieces.

### Rook
- Moves horizontally or vertically any number of steps without jumping over pieces.

### Bishop
- Moves diagonally any number of steps without jumping over pieces.

### Queen
- Moves horizontally, vertically, or diagonally any number of steps without jumping over pieces.

### King
- Moves one step in any direction.

## Requirements
Create a command-line application for a chess validator with the following features:

- **Initialize** a chessboard with pieces in their correct positions.
- **Print** the board after initialization.
- **Allow users** to make moves by inputting the start and end positions.
- **Validate** each move:
  - The piece belongs to the current player.
  - The move is valid for that piece.
  - The start and end positions are within the board.
- **Invalid moves** print "Invalid Move" and allow the same player to try again.
- **Valid moves** update the board and print the new board state.

## Input/Output Format
### Input Format
- Each move is entered as `Start_Position End_Position` (e.g., `e2 e4`).
- Input continues until the word `exit` is encountered.

### Output Format
- The initial board state is printed, followed by an empty line.
- After each valid move, the updated board is printed, followed by an empty line.
- For an invalid move, only "Invalid Move" is printed.

### Board Representation
```
BR BN BB BQ BK BB BN BR
BP BP BP BP BP BP BP BP
-- -- -- -- -- -- -- --
-- -- -- -- -- -- -- --
-- -- -- -- -- -- -- --
-- -- -- -- -- -- -- --
WP WP WP WP WP WP WP WP
WR WN WB WQ WK WB WN WR
```
- `W` and `B` represent white and black pieces.
- `P` => Pawn, `R` => Rook, `N` => Knight, `B` => Bishop, `Q` => Queen, `K` => King.
- Empty cells are represented as `--`.

## Expectations
- **Functional correctness**: Ensure that the program properly validates and executes moves.
- **Code readability**: Follow a modular approach and maintain separation of concerns.
- **Extensibility**:
  - Allow new pieces with different move rules.
  - Change existing piece movement rules if required.
  - Modify board size and starting positions.

## Optional Requirements
- Implement unit tests.
- Ensure minimal code changes for future modifications.
- Keep the code flexible for new features.

This project does not require a graphical user interface (GUI).

