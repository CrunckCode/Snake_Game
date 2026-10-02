# Snake Game

The classic Snake game in Python using the built-in `turtle` graphics module.

## How to play
Run `python main.py`. Steer the snake with the **arrow keys**. Eat the blue food to grow and score a point. The game ends ("GAME OVER") if the snake hits the wall (beyond 280 units from the centre) or runs into its own body. The snake cannot reverse directly into itself. Click the window to exit.

## How it works
- `main.py`: creates the 600 by 600 screen, snake, food and scoreboard, binds the arrow keys, and runs the loop every 0.1 seconds: move, check food (within 15 units), check walls, check collisions with the tail.
- `snake.py`: a `Snake` class that holds a list of square segments (starting with three), moves by shifting each segment into the position of the one in front of it and then advancing the head 20 units, grows with `extend()`, and blocks 180-degree turns by checking the current heading.
- `food.py`: a small blue circle that jumps to a random position when eaten.
- `scoreboard.py`: shows the score at the top and the "GAME OVER" message.

## Skills practised
Object-oriented design, list-based movement of a body, collision detection, keyboard events, and a timed game loop.

## Requirements
Python 3 with Tk support (standard on most installs); no extra packages.
