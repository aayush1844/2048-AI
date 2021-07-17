# Playing 2048 game with an Automated Bot.

Bot uses Expectimax search with the depth of 4 to find the best possible move.


# Files Info

direct.py --> Expectimax implementation (main algorithm)

puzzle.py ---> Implementation of game (main file, run this file for demo)

logic.py ----> Implementation of game (backend)

merge_game.py -----> Helper file for merging the matrix

## Run Game

$ python3 puzzle.py

## Human Play
Click the "Bot Play" button to turn to Manual Playing mode.
Click the same button, now turned to "Human Play" to let the bot take control



## Heuristics

(In file direct.py)

I have used a score and a penalty function.

A configuration gets a high score if it follows snake line pattern.

Weights are assigned to individual tiles. You can modify them to get different results.

Penalty is given depending on how many filled tiles are present (more filled tiles => bigger penalty).
