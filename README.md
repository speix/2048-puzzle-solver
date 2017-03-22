# 2048-puzzle
A.I - Implemented Minimax algorithm with ab-pruning using iterative deepening to solve the 2048-puzzle. Each move selection should be under 0.1 seconds.

Injected 5 different heuristics with adjustable weights to evaluate moves:
```
smoothness (Αdjacent tiles should decrease in value but neighbor tiles should be close enough to potentially merge)
monotonicity (Values of the tiles should all either increasing or decreasing along both the left/right and up/down directions)
emptiness (Evaluates each move based on the number of empty cells it generates)
maxvalue (Evaluates each move based on the maximum value a potential merge can generate but do this based on empty cells)
distance (Measures the manhattan distance of the maximum tile from the upper-left corner)
```

## Usage
python GameManager.py

## Results
The agent surpassed the goal of 2048 value tile and got to 4096. Probably with a minor change on strategy, maybe dynamically altering the heuristic weights, it may go even further.

![alt tag](http://www.supergramm.com/media/images/github/results.jpg)
