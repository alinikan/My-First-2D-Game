## Overview

The Runner Game is a fun, simple 2D game created using the Pygame library in Python. In this game, you control a character that must avoid running into enemies (worms and flies). The character can jump to avoid the enemies, and the game features sound effects and background music to enhance the gameplay experience. The game keeps score based on how long you manage to stay alive. If your character collides with an enemy, the game is over and it will display your final score.

## Files

In the root directory, you'll find a single python file:

- `main.py` is the main game script. This file contains all the logic for the game mechanics.

## Graphics and Audio Files

In the `graphics` directory, there are the following subdirectories:

- `Player`: Contains images for the player character's animations.
- `Fly`: Contains images for the fly enemy's animations.
- `snail`: Contains images for the snail enemy's animations.
- `Sky.png`: Background image for the sky.
- `ground.png`: Background image for the ground.

In the `audio` directory, there are two audio files:

- `jump.mp3`: Sound effect played when the player jumps.
- `music.wav`: Background music played during the game.

The `font` directory contains the font used in the game for displaying text:

- `Pixeltype.ttf`: The custom font file used for text in the game.

## How to Play

1. Use the `space` key to make your character jump and avoid the enemies.
2. The longer you stay alive, the higher your score will get.
3. The game ends when your character collides with an enemy.

## Requirements

To run this game, you need Python 3 and Pygame installed on your system.

## How to Run the Game

To run the game, navigate to the directory containing the `main.py` script and run the following command:

**python3 main.py** or **python main.py**

## Game Mechanics

The game mechanics are fairly straightforward. Your character moves continuously from left to right. The enemies (flies and snails) move towards your character from the right side of the screen. Your goal is to avoid colliding with these enemies by jumping over them.

## Code Explanation

The Player class and the Obstacle class represent the player character and the enemies, respectively. These classes contain the logic for the animations, movements, and actions of the player and the enemies. The pygame.sprite.Sprite class is used as a base class for these classes, providing the necessary functionality for dealing with game elements that can move and be drawn on the screen.

The display_score(), obstacle_movement(), and collisions() functions are used to display the score, move the obstacles, and check for collisions, respectively.

The Pygame event loop handles events like key presses and mouse clicks. The pygame.time.set_timer() function is used to trigger USEREVENT events at certain intervals, which are used to create and animate the enemies.

## Enjoy the Game!

That's it! Enjoy playing the Runner Game and see how long you can keep your character alive!
