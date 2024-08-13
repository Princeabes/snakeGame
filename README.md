# Snake Game

A classic Snake game implemented in Java using Swing. The game involves controlling a snake that grows longer as it consumes apples. The objective is to eat as many apples as possible without running into walls or the snake's own body.

## Features

- **Game Controls**:
  - Arrow keys to control the snake's direction.
  - Press `R` to restart the game after a game over.
  - Press `+` to increase the snake's speed.
  - Press `-` to decrease the snake's speed.

- **Game Mechanics**:
  - The snake starts in the center of the screen and moves in the direction specified by the arrow keys.
  - The game ends if the snake runs into a wall or into itself.
  - The score is determined by the length of the snake.

- **Visuals**:
  - The snake is represented by green squares.
  - The apple is represented by a red square.
  - The walls are drawn around the edges of the window.

## How to Run

1. **Clone the Repository**:
```
   https://github.com/princeabes/snake-game-java.git

2. **Compile and Run**:
- Compile the code using a Java compiler:
  ```
  javac SnakeGame.java
  ```
- Run the compiled Java program:
  ```
  java SnakeGame
  ```

3. **Gameplay**:
- Use the arrow keys to control the snake's movement.
- Try to eat as many apples as possible without colliding with the walls or yourself.

## Code Overview

- **`SnakeGame` Class**:
- The main class of the game, extending `JFrame` and implementing `KeyListener`.
- Manages the game loop, controls the snake's movement, detects collisions, and handles user input.

- **Key Methods**:
- `startGame()`: Starts or restarts the game.
- `move()`: Moves the snake in the current direction.
- `checkApple()`: Checks if the snake has eaten the apple and spawns a new apple if needed.
- `checkCollisions()`: Checks if the snake has collided with the walls or itself.
- `paint(Graphics g)`: Draws the snake, apple, and game elements.
- `gameOver(Graphics g)`: Displays a "Game Over" message when the game ends.

- **Event Handling**:
- Implements `KeyListener` to capture and respond to key events for controlling the snake and adjusting game settings.

## Customization

- **Game Speed**: 
- Modify the `delay` variable in the `SnakeGame` constructor to change the snake's initial speed.

- **Window Size**:
- Adjust the `WIDTH` and `HEIGHT` constants to change the game window size.

- **Unit Size**:
- Modify the `UNIT_SIZE` constant to change the size of the snake and apple.

