# Pig - A Die Game

The game uses only one six sided die and is played with 2 or more players. Players take turns rolling the die and tabulating a score according to the rules. The first player to score 100 or more points wins.

In our version of the game, the six-sided die will be simulated by the computer. Additionally, the game can be played against the computer should there only be one player. If there is more than one player, the game is played as a [hotseat](https://en.wikipedia.org/wiki/Hotseat_(multiplayer_mode)) multiplayer game.

## Rules

* There is at least two players playing the game. A two player game may be against another player or against the computer. Three or more player games do not have a computer player to play against.
* There is at most 4 players in a game.
* There is one six-sided die (simulated by the game using a psuedo-random number generator); the faces of the die are numbered 1, 2, 3, 4, 5, and 6. Opposing sides of the die sum to 7 (standard western casino dice).
* The game is turn based. The player who goes first is selected by each player rolling the die once. The players are ordered from in ascending order. If there is a tie between two or more players, the computer can break the tie by arbitrarily assigning that player to a position not less than the position the player rolled.
* Once each player has had a turn in ascending order, the turn returns to the first player.
* Each turn, a player rolls the die.
    * If the player rolls a 1, the player scores nothing that turn and it becomes the next player's turn. The player's overall score does not change because the player has lost the points accrued during their turn.
    * If the player rolls any other number, the value of the die is added to their turn's score as points and the player's turn may continue. The player's overall score does not change until their turn ends.
    * If a player chooses to hold, their turn total is added to their score, and it becomes the next player's turn.
* The play may not choose to hold until after the die has been rolled at least once.
* The game ends when a player ends their turn with a score of 100 points or greater.
* At the beginning of every die roll, the game displays the current player's total score, current turn score, and how many times the player has rolled. Once the die is rolled, the computer displays the value of the die. If it is a 1, the computer ends the current player's turn and moves on to the next player.
