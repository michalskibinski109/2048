# Game2048

Game2048 is a Python implementation of the popular game 2048. It provides a console-based interface for playing the game and supports different player types, including human, AI, and random players.

## Installation

To use the Game2048 module, you need to have Python 3.x installed. You can install the required dependencies using pip:

```shell
pip install numpy easy_logs
```

## Usage

Here is an example of how to use the Game2048 module:

```python
from game2048 import Game2048

game = Game2048()
game.play_in_console(sleep_time=0.5, player="human")
```

In the above example, a new instance of the `Game2048` class is created, and the `play_in_console` method is called with a sleep time of 0.5 seconds and the player set to "human". The `play_in_console` method starts the game in the console, allowing the player to make moves by entering the desired direction using the keyboard.

### Player Types

The `play_in_console` method supports different player types:

- **human**: Allows a human player to make moves using the keyboard. The player needs to enter the direction (w, a, s, or d) for each move.

- **ai**: Uses an AI player based on the minimax algorithm to find the best move for each turn.

- **random**: Makes random moves for each turn.

You can choose the player type by setting the `player` parameter when calling the `play_in_console` method.

## Documentation
Code documentes itself. 
after running the code:
```python
print(Game())
```
you will get the following documentation:
```
Game:
        Supported algorithms:
            - minimax
        Future algorithms:
            - Reinforcement Learning
            - Monte Carlo Tree Search
            - Expectimax


Board:

    Rules:
        - The board is a N x M grid (defined by `shape` argument)
        - The game starts with two tiles with values 2 or 4
        - The player can move the board in four directions: up, down, left, right
        - If two tiles with the same value collide while moving, they merge into a new tile
        - The value of the new tile is the sum of the two tiles that collided
        - After each move, a new tile with value 2 or 4 appears on the board
        - The player wins when a tile with value 2048 appears on the board
```

## Dependencies

The Game2048 module relies on the following dependencies:

- `numpy`: Used for numerical operations and generating random numbers.

- `easy_logs`: Provides logging capabilities.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.