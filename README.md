Spaceship Adventure
--------------------------------------

Spaceship Adventure is a side scrolling shoot
the bad guy starter kit.  It can be any game
you want.  Use your imagination to design
something great, then figure out how to change
the code to put your design into action.

The starter kit has a side scrolling layout where
the player is on the left of the screen, and the
opponents approach from the right side of the
screen.

In the starter kit, the player can move up and
down the screen, as well as 1/3 of the way to the
right.  The opponents are generated on the right
side of the screen at random positions vertically.
The opponents are generated about 2 per second.
The player can shoot bullets that travel left to
right as fast as they can press the space bar.
If a bullet collides with an opponent, the bullet
and the opponent are destroyed.  If the bullet
reaches the right side of the screen, it is 
destroyed.

In the code, the player is referred to as the
spaceship.  The opponents are referred to as
baddies.  The bullet is referred to as a bullet.

This does not mean that your game must be a 
spaceship fighting aliens that scroll from 
right to left.  You can use any theme or idea
for your game.  You are encouraged to use your
creativity to take this starter code and create
something fun and interesting.


Requirements
--------------------------------------

- Python3
- Pygame

If you are new to programming with Python, then
we recommend you install [Thonny](https://thonny.org/).
Once Thonny is installed, start it up, go to 
Tools->Manage Packages, find and install Pygame.
From there, unzip the starter code, read the
brief introduction below, and get to work.


The Code
-----------------------------------------

main.py:
  This is where the screen size and frame rate
are configured.  The rest of this code should
not need to be changed.

SpaceshipAdventure.py:
  This is where the message in the title bar of
the window is configured.  The rest of this code
should not need to be changed.

SpaceshipData.py:
  This is the most complicated part of the code.
It configures the overall display and gameplay.

  \_\_init\_\_():
    Used to configure the size, speed and color
  of the spaceship; size and color of bullets;
  and size and color of the baddies.

  evolve():
    Used to configure the keys that move the ship
  and fire bullets;  randomly create more baddies;
  move bullets; move baddies; remove bullets that
  hit the right side; remove baddies that hit the
  left side; remove bullets and baddies that collide.

  addBaddie():
    Used to generate random location for new baddie.

  draw():
    Used to display the entire game display, including
  the background.

spaceship.py:
  This is where the spacehip's behavior and display
are configured.

baddie.py:
  This is where the baddies' behavior and display
are configured.

bullet.py:
  This is where the bullets' behavior and display
are configured.

game_mouse.py:
  This file does basic setup of the window, and
receives mouse and keyboard events, then sends
the events to the game code.  The code in this
file should not need to be changed.



Short list of possible tasks to customize
-----------------------------------------
- Change the color of the ship/bullets/baddies
- Change the shape of the ship/bullets/baddies
- Change the ship/bullets/baddies to be images
- Add a score keeping system to track the number
  of baddies killed.
- Display the score.
- Add a lives system to track the number of baddies
  that have escaped.
- End the game when there are no more lives left.
- Display the number of lives left.
- Have the ship die if it collides with a baddie.
- Organize waves of baddies.
- Give baddies organized patterns.
- Let the baddies shoot.
- You think of something cool.

Partial Instructions
--------------------

- [Add Music](2022_add_music.md)
- [Add Sounds](2022_add_sound.md)
- [Add Images](2022_add_images.md)
- [Add Score](2022_add_baddie_score.md)
- [Add Tougher Baddies](2022_add_baddie_hit_points.md)

