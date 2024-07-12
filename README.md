Dice Game

This Python script implements a simple dice game for 2 to 4 players. Players take turns rolling a die, accumulating points unless they roll a 1, which ends their turn. The first player to reach or exceed a score of 50 wins the game.

Getting Started

Prerequisites

- Python 3.x installed on your system

Running the Game

1. Save the script to a file, for example, `dice_game.py`.
2. Open a terminal or command prompt.
3. Navigate to the directory where the script is saved.
4. Run the script using the command: `python dice_game.py`.

Game Rules

1. The game requires 2 to 4 players.
2. Players take turns to roll a die.
3. On each turn, a player can roll the die as many times as they wish.
4. The player accumulates points equal to the die roll.
5. If the player rolls a 1, their turn ends, and they score no points for that turn.
6. The first player to reach or exceed a score of 50 wins the game.

Code Overview

Functions

- `roll()`: Simulates rolling a die and returns a random integer between 1 and 6.

Main Logic

1. The script prompts the user to enter the number of players (between 2 and 4).
2. It initializes the scores for all players to 0.
3. The game enters a loop where players take turns until one player's score reaches or exceeds 50.
4. During a player's turn:
    - They are prompted to roll the die.
    - If they roll a 1, their turn ends, and they score no points for that turn.
    - Otherwise, the rolled value is added to their current turn's score.
    - The player can choose to roll again or end their turn.
5. The player's score for the turn is added to their total score.
6. The game checks if any player has reached or exceeded the winning score.
7. The game announces the winner and their score.

Example Output

```
Enter the number of players: 3

 Player number 1 turn has just started!

Your total score is: 0

Would you like to roll (y)? y
You rolled a: 4
Your score is: 4
Would you like to roll (y)? y
You rolled a: 5
Your score is: 9
Would you like to roll (y)? n
Your total score is: 9

 Player number 2 turn has just started!

Your total score is: 0

Would you like to roll (y)? y
You rolled a: 3
Your score is: 3
Would you like to roll (y)? y
You rolled a: 1
Your rolled a 1! Turn done!
Your total score is: 0

...

Player number 1 is the winner with score of: 50
```
