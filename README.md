# Flappy Bird Game Documentation

## Introduction
This document provides documentation for the Flappy Bird game implemented in Python using the Pygame library. The game is a simple side-scrolling arcade game where the player controls a bird that must navigate through a series of pipes without colliding with them.

## Prerequisites
Before running the game, make sure you have Python installed on your system. Additionally, install the Pygame library using the following command:
```bash
pip install pygame
```

## Game Components

### 1. Main Script (`flappy_bird.py`)
This script contains the main game logic and functions. The key components are:
- **Global Variables**
  - `FPS`: Frames per second for controlling the game speed.
  - `SCREENWIDTH` and `SCREENHEIGHT`: Width and height of the game window.
  - `GROUNDY`: Y-coordinate of the ground in the game.
  - `GAME_SPRITES`: Dictionary to store game sprites.
  - `GAME_SOUNDS`: Dictionary to store game sounds.
  - `PLAYER`, `BACKGROUND`, `PIPE`: File paths for player, background, and pipe sprites.

- **Functions**
  - `welcomeScreen()`: Displays the welcome screen with instructions and waits for the user to start the game.
  - `mainGame()`: Contains the main game loop and logic, including player movement, pipe generation, collision detection, and scoring.
  - `isCollide()`: Checks if the player collides with the ground or pipes.
  - `getRandomPipe()`: Generates random pipe positions for blitting on the screen.

- **Game Initialization**
  - Pygame is initialized, and necessary resources (sprites, sounds) are loaded.
  - The game window is set up with a title.

- **Game Loop**
  - The script continuously runs the `welcomeScreen()` and `mainGame()` functions in an infinite loop.

### 2. Sprites and Sounds
- **Sprites**: The game includes images for the player, pipes, background, base, and numbers (for score display).
  - Player sprite: `'gallery/sprites/bird.png'`
  - Background sprite: `'gallery/sprites/background.png'`
  - Pipe sprite: `'gallery/sprites/pipe.png'`
  - Base sprite: `'gallery/sprites/base.png'`
  - Number sprites: `'gallery/sprites/0.png'` to `'gallery/sprites/9.png'`

- **Sounds**: The game includes sound effects for various events.
  - `'gallery/audio/die.wav'`: Player collision sound
  - `'gallery/audio/hit.wav'`: Pipe hit sound
  - `'gallery/audio/point.wav'`: Score point sound
  - `'gallery/audio/swoosh.wav'`: Wing swoosh sound
  - `'gallery/audio/wing.wav'`: Wing flap sound

## Running the Game
1. Execute the script `flappy_bird.py` using Python:
   ```bash
   python flappy_bird.py
   ```
2. The game window will appear, displaying the welcome screen.
3. Press the spacebar or up arrow key to start the game.
4. Control the bird's movement by pressing the spacebar or up arrow key to avoid pipes.
5. The game ends if the bird collides with the ground or pipes.

## Dependencies
- Python 3.x
- Pygame library

## Credits
- Original Flappy Bird game concept by Dong Nguyen.
- Python implementation by Rupak Verma.

## License
This Flappy Bird game implementation is provided under the [MIT License](LICENSE). Feel free to modify and distribute it as per the terms of the license.
