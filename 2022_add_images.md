Adding Images to Pygame Programs
-------------------------------

I'm going to replace the rectangles for objects in my game
with images, to add more interesting visuals.

Image Files
-----------

First, I need to make or find a suitable image file. There are many
image file formats.  Pygame supports many of them, but it depends
on your computer system installation.  It's best to get your
image and try it.  If the file doesn't work, convert to another
format and try again.

I've had most success with PNG and JPG files for images.

It is important to keep in mind the size of the rectangles
on the screen while looking for or creating image files.
I can see in `SpaceshipData.py` that my spaceship is 20
pixels wide and 10 pixels high. So, I'm looking for a spaceship
that is twice as wide as it is tall.

I found my spaceship image file and named it `spaceship.png`.
it turns out the image is 40 pixels wide and 26 pixels
tall. I'll make adjustments for that.


Loading the Image File
----------------------

Next, we'll need to load the image file into the program
so we can display it.  This needs to be completed in 
Spaceship's \_\_init\_\_ method.  Here are the lines I would 
put, right after the line that initializes the color.

    self.image = pygame.image.load("spaceship.png")
    
Notice the name of the image file is in quotes.  This
name must match the file name exactly.  If your operating
system hides the file extension, be sure that you have it
correct.

You should check your program for syntax errors before proceeding.


Showing Images
---------------

Now that the image file is loaded into the program, we need to
make it display instead of drawing the ship's solid color
rectangle.

This needs to be completed in SpaceShip's draw
method.  Remove the lines that create and display a 
rectangle for the ship, and replace it with this
line that displays the image instead:

    surface.blit(self.image, (self.x, self.y))

You should check your program for syntax errors before 
proceeding.

Run the program.  You should see the image instead
of a solid rectangle for the spaceship.

Correcting the Spaceship Size
-----------------------------

In order for the spaceship to behave in a way that makes
sense with the image, we need to make the size of the
spaceship match the size of the image. This is done
in SpaceshipData's \_\_init\_\_ method. Find the
location were the spaceship's width and height are
set, and change the numbers to match the image size.
For me this looks like:

    self.spaceship_width = 40
    self.spaceship_height = 26


Bullets and Baddies
-------------------

These same ideas can be used to make images for bullets and baddies.

Tips
----

The spaceship is on the left side of the screen, and shoots to the
right. Use and image that has the nose of the ship on the right side
for best appearances. 

The bullet comes from the center of the spaceship's right side. Have
the nose of the spaceship near the middle of the image.

Learning More About Music in Pygame
------------------------------------

* [Image Documentation](https://www.pygame.org/docs/ref/image.html)







