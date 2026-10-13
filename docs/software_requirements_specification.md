# Overview
The purpose of this document is to outline the software requirement specifications of the 2D platformer game. This document will outline the functional and non-functional requirements to be met when creating the game.

# Functional Requirements
1. Player Movement
    1. M1: When the user presses and holds either the Up Arrow key or the ‘W’ key, the player avatar shall move upward along the Y-axis at the designated movement speed until the key is released.
2. Level/Stage
    1. S1: The game stage shall scroll automatically along the positive X-axis from (0, 0) to (1150, 0) at a constant velocity of 100 pixels per second, while background layers loop seamlessly via Parallax2D.
    2. S2: The player character's collision boundaries shall resolve contact with all static environment meshes to prevent visual intersection.
    3. S3: The game shall terminate the level immediately when the player avatar’s Y-coordinate becomes less than -500 pixels.

# Non-Functional Requirements
1. Peformance
    1. P1: The game engine shall maintain a minimum framerate of 60 frames per second on a Window 11 OS desktop at 1080p resolution.
    2. P2: The initial loading screen between main menu and gameplay stage shall be completed in less than 5 seconds.
    3. P3: The game shall not exceed  4 GB of maximum runtime memory allocation during continuous level execution.
2. Compatibility
    1. C1: The source code and project architecture shall be fully compatible with GODOT 4.7.2 without requiring custom engine source recompilation.