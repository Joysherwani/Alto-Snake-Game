# Alto-Snake-Game

1. Introduction
"This is a simple Snake Game created using Python's Tkinter module. The objective of the game is to control a snake, eat food to grow longer, and avoid colliding with the walls or itself."

2. Technologies Used
Python: The programming language used.

Tkinter: A built-in Python GUI library used for rendering graphics.

Random module: Used to generate food at random positions.

3. How the Game Works
The snake moves continuously in the direction chosen by the arrow keys.

The food is placed randomly on the screen.

When the snake eats the food, its length increases, and the score goes up.

The game ends if the snake collides with the wall or itself.

4. Key Features in the Code
a) Game Window Setup
Created using Tkinter, with a black canvas of 625x625 pixels.

The window is centered on the screen.

b) Game Objects (Snake and Food)
The snake and food are represented by a Tile class with x and y coordinates.

The snake starts with one tile and grows when it eats food.

c) Game Logic
Snake Movement: Controlled using the change_direction(e) function.

Collision Detection:

If the snake hits the wall, game_over = True.

If the snake hits itself, game_over = True.

Eating Food:

If the snake reaches the food's position, it grows, and the food is repositioned.

d) Game Loop
The game runs in a loop using window.after(100, draw), updating the screen every 100 milliseconds (10 FPS).

The draw() function:

Clears the screen.

Redraws the food and snake.

Displays the score and Game Over message if needed.
