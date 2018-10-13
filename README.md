# Transformations

This Exercise describe openGL with C++ Transformation (translation ,Rotation,Scale) ,Color and PUSH and POP Operations .

 
# Color 
use built in function 
glColor3f (float ,float ,float ) to change of vertics or an object 
use glclearcolor ( float ,float ,float ) to change backgroud color 

parameters are (Red , green ,blue)
RGB is a very common way to represent colors on computers. Using the RGB system, we specify each color as a combination of red, blue, and green light components, where each component ranges from 0 to 1.


# Translation

We translate by using a call to glTranslatef, with the amount that we want to translate in the x, y, and z directions.
gltranslatef use to move the center of drawing (orgin) to the coordinates specified then draw any shape .

glTranslatef(1.0f, 0.0f, 0.0f); // move 1 in positive X
glTranslatef(0.0f, 0.0f -5.0f); // use the translation here to make shape easy to see by move it in negative Z ( as expand your hand in front of you to can read easily)

# Rotation
We introduced a new variable, angle, which stores the number of degrees by which we want to rotate our shapes. We also use two new functions. We call glRotatef, which rotates our shape. 

glRotatef(angle, 0.0f, 0.0f, 1.0f)   // rotates our shape by angle degrees about the z-axis
glRotatef(_angle, 1.0f, 2.0f, 3.0f) //rotates our bird by _angle degrees about the vector (1, 2, 3).


# Scale
glScalef(0.7f, 0.7f, 0.7f) which shrinks our bird to 70% of its original size in the x, y, and z directions. 
If we were to call glScalef(2.0f, 1.0f, 1.0f) instead, we would double its size in the horizontal direction, according to its perspective.

# push & pop
There are two new and important functions used in this code: glPushMatrix() and glPopMatrix(). We use them to save and restore the state of our shape. 
glPushMatrix saves its state, and glPopMatrix restores .
