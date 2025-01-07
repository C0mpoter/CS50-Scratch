# Circuit Crawl: A Python Snake Game with Obstacles and Energy Nodes

## Overview

**Circuit Crawl** is a Python-based snake game where the player controls a snake, collects energy nodes to grow in size, and avoids obstacles that appear randomly on the screen. The game ends when the snake collides with itself, a wall, or an obstacle. At the end of the game, a death screen is displayed, showing the player's score along with the high score. The player can either replay the game or quit.

This game was developed using the **Pygame** library and is intended to provide an engaging experience for both novice and experienced players alike, with simple mechanics, but the added complexity of growing the snake and avoiding randomly placed obstacles. The game provides a basic interface, showing real-time score updates, with smooth movement mechanics and a functional game-over screen with options for replaying or quitting.

## Project Structure

### Files Included:

1. **Main Game Script (`main.py`)**:
   - This is the primary script where the game logic and user interface are implemented. It contains all the functionality of the game, including snake movement, collision detection, energy collection, obstacle handling, score tracking, and the game-over screen.
   - The script uses the **Pygame** library to create the graphical user interface and to handle user input via keyboard for snake movement.
   - The `main.py` file includes a game loop that runs continuously until the player either loses the game or chooses to quit. The game supports key input (arrow keys) to control the snake’s movement and has a delay mechanism to control the snake’s speed. Upon collision with an obstacle or the snake itself, a "Game Over" screen appears, showing the player's score and the high score, with options to replay or quit.

2. **Game Assets (No external assets included)**:
   - This project does not rely on external images or sound files. The game uses basic Pygame shapes (rectangles) for the snake, obstacles, and energy nodes. The game’s aesthetic is minimalist but functional.

## Key Features

### Snake Mechanics:
- The snake starts at the center of the screen and moves in one of four directions (up, down, left, right) based on the player's input.
- The snake grows in length each time it collects an energy node, which spawns randomly on the screen.
- If the snake collides with itself, the walls, or obstacles, the game ends, and the player is presented with a death screen showing their score and the high score.

### Obstacles and Energy Nodes:
- **Energy Nodes**: These are randomly placed on the screen. When the snake eats an energy node, it grows in size, and the score increases.
- **Obstacles**: These appear randomly on the screen and are deadly to the snake. If the snake collides with an obstacle, the game ends.
  
### Death Screen:
- Upon the game’s conclusion, the death screen is displayed, showing:
  - The **current score** the player achieved in the current session.
  - The **high score**, which persists across game sessions.
  - Two buttons allowing the player to either **Replay** the game or **Quit**.
  - The buttons are implemented with mouse interaction, and clicking them triggers the corresponding actions.
  
### High Score Tracking:
- The game tracks the highest score the player has achieved during the game sessions. When a player achieves a new high score, it is updated and displayed on the death screen.
  
### User Interface:
- The main game screen displays the snake, obstacles, energy nodes, and the player’s score in real-time.
- The death screen is simple and includes options to replay or quit the game.
  
## Design Choices and Considerations

### Why Pygame?
I chose **Pygame** for this project due to its simplicity and efficiency in handling 2D game mechanics. Pygame provides excellent libraries for handling graphics, user input, and game loop management, making it ideal for a beginner-friendly game like Snake. While other game engines like Unity or Godot are more powerful, they are more complex and not necessary for a simple 2D game like this one. Pygame also allows for quick development and prototyping.

### Snake Movement Delay:
To avoid the snake becoming too fast or erratic, I introduced a **movement delay** that regulates how frequently the snake can move. The delay is measured in milliseconds, and by controlling the timing, the game can ensure that the snake moves at a consistent speed, which is crucial for player control and gameplay balance.

### High Score Tracking:
The high score is maintained across multiple sessions by saving the highest score in memory. This design allows for better player engagement, as it gives players a sense of accomplishment when they surpass their previous high score. It also introduces a competitive element to the game, encouraging players to improve with each attempt.

### Game Over Screen:
The game-over screen provides clear and simple options for the player to either replay the game or quit. I decided on a minimalist design for the screen, showing just the relevant information (score, high score) and two buttons for actions. This ensures that the player can quickly see their performance and choose what to do next without any unnecessary distractions.

### Button Design:
The buttons on the death screen are interactive, with hover effects to provide visual feedback to the player. The buttons are designed to be simple and straightforward, with "Replay" and "Quit" options placed below the score text to avoid visual clutter.

### Obstacle Placement:
Obstacles spawn randomly on the screen, and their placement adds difficulty to the game as the player progresses. This randomness keeps the gameplay fresh and unpredictable, as each session will be slightly different due to the random placement of obstacles and energy nodes.

## Conclusion

**Circuit Crawl** is a simple yet engaging snake game created using Python and Pygame. The project demonstrates the power of Pygame in handling basic game mechanics, including user input, collision detection, and real-time score tracking. By incorporating obstacles, energy nodes, and a death screen with replay options, the game offers an entertaining and user-friendly experience. Although the current version is minimalistic, the game provides a strong foundation for further enhancement and additional features.

I am proud of this project as it serves as both an enjoyable game and a great learning experience in Python game development. It has helped me understand the importance of smooth game mechanics, user interface design, and gameplay balance. The experience gained from developing this game will be invaluable for future projects.
