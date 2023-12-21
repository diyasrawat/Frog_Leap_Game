# Frog_Leap_Puzzle_Game

# Overview:
The Frog Leap Puzzle Game is a Python implementation of a classic console-based puzzle where two sets of frogs, one green and one brown, are placed on opposite sides of a river. The objective is to swap the positions of the green and brown frogs using specific movement rules until they are in the opposite arrangement.

# Features:
Frog Types:

Green frogs ('G') move exclusively to the right.
Brown frogs ('B') move exclusively to the left.

# Movement:

Frogs can advance one space forward.
A frog can leap over another frog from the opposite set, given there is an empty space beyond the leaped frog.

# Objective:

The puzzle is solved when the green frogs are positioned on the right side, and the brown frogs are on the left side.

**How to Play:**

**Initial State:**

The game starts with an initial configuration of frogs, represented by 'G' and 'B', and an empty space on the board.

**User Input:**

Players interact by entering an integer between 0 and 6, corresponding to the position of a frog they wish to move.
Input options also include 'q' to quit the game or 'r' to restart with a fresh puzzle.

**Valid Moves:**

Green frogs move to the right if there is an empty space or if they can leap over a brown frog.
Brown frogs move to the left if there is an empty space or if they can leap over a green frog.

**Game State:**

After each move, the current state of the game board is displayed, illustrating frog positions and the empty space.

**Game Completion:**

Victory is achieved when the frogs mirror the opposite order of their initial positions (['B', 'B', 'B', '-', 'G', 'G', 'G']).
Players can opt to end the game ('q').

**Restart Option:**

Upon completion or quitting, players have the choice to restart by entering 'r'.

**End the Game Loop:**

If players choose to end the game loop ('e') during play, the game loop gracefully exits.

# Usage:

To play the game:

Run the script.
Enter an integer between 0 and 6 to move a frog, 'q' to quit, 'r' to restart, or 'e' to end the game loop.

# Explanation

    class FrogLeapGame:
    """
    Class representing the Frog Leap Puzzle Game.

    Attributes:
    - positions (list): List representing the current positions of frogs and the empty space.

    Methods:
    - __init__(self): Initializes the game with the starting positions of frogs.
    - print_board(self): Prints the current state of the game board.
    - make_move(self, position): Processes the user's move based on the selected frog position.
    - check_win(self): Checks if the current positions constitute a win.
    - restart(self): Restarts the game with a new initial configuration.
    - end_game(self): Ends the game loop.

    """

    def __init__(self):
        """
        Initializes the Frog Leap Puzzle Game.

        The initial configuration of frogs is ['G', 'G', 'G', '-', 'B', 'B', 'B'].

        """
        self.positions = ['G', 'G', 'G', '-', 'B', 'B', 'B']

    def print_board(self):
        """
        Prints the current state of the game board.

        Displays the positions of frogs and the empty space.

        """
        print("[ 0 ,  1 ,  2 ,  3 ,  4 ,  5 ,  6 ]")
        print(self.positions)

    def make_move(self, position):
        """
        Processes the user's move based on the selected frog position.

        Parameters:
        - position (int): The position of the selected frog.

        """
        # Implementation of frog movement rules and position swapping goes here

    def check_win(self):
        """
        Checks if the current positions constitute a win.

        Returns:
        - bool: True if the game is won, False otherwise.

        """
        # Implementation to check if the current positions constitute a win goes here
        return False

    def restart(self):
        """
        Restarts the game with a new initial configuration.

        """
        # Implementation to reset the game to its initial configuration goes here

    def end_game(self):
        """
        Ends the game loop.

        """
        # Implementation to end the game loop goes here


# Notes:
The game is designed for console-based play, providing a simple yet enjoyable environment for solving the Frog Leap Puzzle.
