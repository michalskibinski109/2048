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


| Player Type | Description                                                                                                                            |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| `human`     | Allows a human player to make moves using the keyboard. The player needs to enter the direction (`w`, `a`, `s`, or `d`) for each move. |
| `ai`        | Uses an AI player based on the minimax algorithm to find the best move for each turn.                                                  |
| `random`    | Makes random moves for each turn.                                                                                                      |

You can choose the player type by setting the `player` parameter when calling the `play_in_console` method.

## Dependencies

The Game2048 module relies on the following dependencies:

- `numpy`: Used for numerical operations and generating random numbers.

- `easy_logs`: Provides logging capabilities.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.