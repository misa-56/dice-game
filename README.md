# dice-game
Dice Game

Write a dice game by script that accepts N number of players and M number of dice as input
dice, with the following rules:
1. At the start of the game, each player gets a dice of M units.
2. All players will roll their respective dice at the same time
3. Each player will check the results of their roll of the dice and evaluate as follows:
a. Dice number 6 will be removed from the game and added as points for the player.
b. Dice number 1 will be awarded to the player sitting beside him. For example, the first player will give the dice the number 1 to the second player.
c. Dice numbers 2,3,4 and 5 will still be played by the player.
4. After the evaluation, the player who still has the dice will repeat the 2nd step
until only 1 player remains. Players who have no more dice are considered to have finished playing.
5. The player who has the most points wins.
The number of Players and Number of Dice can be typed input.

Example:
Player = 3, Dice = 4
====================
Turn 1 roll the dice:
Player #1 (0): 3,6,1,3
Player #2 (0): 2,4,5,5
Player #3 (0): 1,2,5,6
After evaluation:
Player #1 (1): 3,3,1
Player #2 (0): 2,4,5,5,1
Player #3 (1): 2,5
====================
Turn 2 roll the dice:
Player #1 (1): 1,2,6

Player #2 (0): 4,3,1,3,3
Player #3 (1): 1,6
After evaluation:
Player #1 (2): 2,1
Player #2 (0): 4,3,3,3,1
Player #3 (2): 1
====================
Turn 3 roll the dice: Player #1 (2): 6,1
Player #2 (0): 2,5,6,4,6
Player #3 (2): 1
After evaluation:
Player #1 (3): 1
Player #2 (2): 2,5,4,1
Player #3 (2): _ (Stop playing because it has no dice)
====================
Turn 4 roll the dice:
Player #1 (3): 1
Player #2 (2): 3,4,5,5
Player #3 (2): _ (Stop playing because it has no dice)
After evaluation:
Player #1(3): _ (Stop playing for not having dice)
Player #2 (2): 3,4,5,5
Player #3 (2): _ (Stop playing because it has no dice)
====================
Game ends because only player #2 has dice.
Game won by player #1 because it has more points than other players
