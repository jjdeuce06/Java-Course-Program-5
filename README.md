# Java-Course-Program-5
This program is an extension of program 4, meaning That everything in program 4 is in this program as well
Please see my Java-Course-Program-4 repo that describes the entirety of the Bounce program
This repo will discuss the extensions my group and I added

## Program Overview
This program adds the use of rectangles for the ball. The user is allowed to click and drag a rectangle onto the screen, as long as the ball is not within that rectangle. The user may double click on the rectaqngle to remove it from the screen

## Implementation (new things only)
- import the Vector class in order to easily add/delete rectangles
- extend MouseListener and MouseMotionListener
- run()
  - add a call to the checkRec() function
- mouseClicked()
  - create a point and set it to the position the user clicked
  - create a new rectangle named deletecheck
  - begin a while loop with counter i
    - set deletecheck to the current vector position
    - if the point is within this rectangle, delete the rectangle
    - traverse the entire Vector. any rectangles within this point are deleted
- mousePressed()
  -  set point m1 to the position the user clicked
- mouseReleased()
  - set good flag to true
  - set index i to 0, get half the ball size, and create new rectangles
  - check if the ball intersects with the rectangle
    - if so, set good to false
    - reset the bounds of the rectangle
    - set the dragbox to 0
    - repaint
  - begin a do while loop
  - if the index is 0, add the rectangle to the vector
  - set the grab variable and get the first rectangle in the vector
  
