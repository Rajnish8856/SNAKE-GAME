# SNAKE-GAME
*COMPANY NAME*:CODTECH IT SOLUTIONS
*NAME*:RAJNISH
*INTER ID*:CT04DF209
*DOMAIN NAME*:C++
*DURATION*:4 WEEKS
*MENTOR*:NEELA SANTOSH KUMAR
#DESCRIPTION OF CODE
This Snake Game is a classic implementation of the well-known retro arcade game, developed using the Simple and Fast Multimedia Library (SFML). It features clean object-oriented design, basic graphics rendering, keyboard input handling, and audio playback to create an interactive and engaging gameplay experience.

The game takes place in a fixed-size window of 800x600 pixels, with the snake moving across a grid where each cell measures 20x20 pixels. The player controls the snake using the arrow keys on the keyboard. The primary goal is to guide the snake to eat food items, which appear randomly on the screen, thereby increasing the snake’s length and the player's score.

The core of the game is managed by a single class, SnakeGame, which encapsulates all game logic, rendering, and event handling. The run() function controls the main game loop. It continuously processes user inputs, updates the game state at regular intervals based on a timer, and renders all visual elements to the window. The game loop only updates the snake’s movement when a set amount of time has passed, effectively controlling the snake's speed.

The snake itself is represented as a vector of sf::Vector2f positions. Each segment of the snake is drawn as a green rectangle, and its movement is implemented by shifting the position of each segment to follow the one ahead of it. This mimics the appearance of a growing and slithering snake. The direction of movement is controlled through keyboard inputs, ensuring that the snake cannot reverse into itself directly.

Food items are rendered as red circles using sf::CircleShape. When the snake’s head collides with a food item, the snake grows by one segment, the player’s score increases, and a new food item is spawned at a random location. To avoid overlapping food with the snake, a check ensures that food is not spawned on any existing segment.

The game includes collision detection for walls and self-collisions. If the snake's head touches the boundary of the window or any part of its own body, the game ends, triggering a game-over screen. The player can restart the game by pressing the ‘R’ key, which resets the score, snake position, and game state.

Audio elements enhance the user experience. Background music plays in a loop throughout the gameplay, and sound effects are triggered when the snake eats food or the game ends. These are handled using sf::Music and sf::Sound from the SFML audio module, with the respective sound files loaded at initialization.

A score counter is displayed at the top-left of the screen using sf::Text, giving the player real-time feedback. The font is loaded from an external file, and the score text is updated continuously as the game progresses.

The snake’s speed increases dynamically with the score, providing a progressive challenge to the player. This is achieved by reducing the time interval between updates as the score increases, with a lower bound to prevent the game from becoming unplayable.

Visually, the game is minimalist but effective, utilizing simple shapes and colors for clarity and ease of understanding. The code is designed with modularity and readability in mind, making it easy to extend with new features such as high score tracking, obstacles, or custom skins.

In conclusion, this Snake Game using SFML demonstrates how a simple 2D game can be developed using C++ and multimedia libraries. It covers essential game development concepts like real-time input handling, collision detection, timed updates, basic UI rendering, and audio feedback, making it a solid starting point for beginners and a useful project for learning game programming.
