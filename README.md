# Conways-Game-of-Life
# Author : Saket Savarn (outcastdreamer)

This code works in python 3.x and for both platforms Linux and Windows.
Conway's game of life is a zero player game played by the computer itself and follows the concept of cellular automata. 
This code is the miniature version of the famous game whose law where stated by [John Conway](https://en.wikipedia.org/wiki/John_Horton_Conway)
who is also a celebrated mathematician.

Click [here](https://www.youtube.com/watch?v=ouipbDkwHWA&t=135s) to understand the rules and the working of the game and
also check this [video](https://www.youtube.com/watch?v=C2vgICfQawE&t=98s) out to see the game in live action and to see the
full version of the game.

My code follows the coordinate system to track each box or cell and it's status.
It starts from negative X-axis coordinate and goes on to positive X-axis coordinate of the same magnitude.
The same applies for Y-axis which also has the same magnitude as X-axis corner/edge coordinates.


Imagine each of these to be boxes/grids/cells, then the demonstration of each cell for X & Y axis ranging from -10 to 10 is :
Here, (-10,10) is cell no. 1, (-9,10) is cell no. 2 and so on.

  **(-10,10)** (-9,10) (-8,10) (-7,10)............(-2,10) (-1,10) ( 0,10) ( 1,10) ( 2,10)............... ( 9,10) **( 10,10)**
  (-10, 9) (-9, 9) (-8, 9) (-7, 9)............(-2, 9) (-1, 9) ( 0, 9) ( 1, 9) ( 2, 9)............... ( 9, 9) ( 10, 9)
  (-10, 8) (-9, 8) (-8, 8) (-7, 8)............(-2, 8) (-1, 8) ( 0, 8) ( 1, 8) ( 2, 8)............... ( 9, 8) ( 10, 8)
  .
  .
  .
  .
  .
  .
  .
  (-10, 0) (-9, 0) (-8, 0) (-7, 0)............(-2, 0) (-1, 0) **( 0, 0)** ( 1,10) ( 2, 0)............... ( 9, 0) ( 10, 0)
  (-10,-1) (-9,-1) (-8,-1) (-7,-1)............(-2,-1) (-1,-1) ( 0,-1) ( 1,-1) ( 2,-1)............... ( 9,-1) ( 10,-1)
  (-10,-2) (-9,-2) (-8,-2) (-7,-2)............(-2,-2) (-1,-2) ( 0,-2) ( 1,-2) ( 2,-2)............... ( 9,-2) ( 10,-2)
  .
  .
  .
  .
  .
  .
  (-10,-9) (-9,-9) (-8,-9) (-7,-9)............(-2,-9) (-1,-9) ( 0,-9) ( 1,-9) ( 2,-9)............... ( 9,-9) ( 10,-9)
  **(-10,-10)** (-9,-10) (-8,-10) (-7,-10)............(-2,-10) (-1,-10) (0,-10) (1,-10) (2,-10)............... (9,-10) **(10,-10)**
  
Here, the total no. of coordinates on X and Y axis are 21 each.{First from -10 to -1 is 10, then 0 to 10 is 11, so 10+11=21 in total).
Hence the total no. of cells/boxes/grids = 21 x 21 = 441 in this case. 

**Note :** 
1) -10 value for X-axis and 10 for Y-axis is the best in terms of CPU performance. (when the code asks you to input values for X and Y axis)
2) After you input the range for creating the total no. of boxes, you will be asked to input selection method for life-cells
   this refers to which life cells do you want in the begining of the game to start the game.
3) Choosing option "1" runs pre-selected Life-cells whose coordinates are already stored in the code. 
4) Choosing option "2" asks for number of cells you would want to be randomly alive in the beginning where the range is from 10 to total no. of boxes.
   By experimentation I have found out that 1/3rd of total no. of boxes (or less than 1/3rd) give the best result.
   If total no. of boxes = 441, then 147 is a good value. Entering values which are 400+ in this case leads to over-population of live cells and fast killing (almost like a genocide :P)
5) Choosing option "3" allows you to input your own coordinates of life-cells. This option is useful to check specific conditions like the "glider" or such recognizable patterns in Game of Life.
   The range for this option is valid for all edge coordinates only (-10 to 10 in above example).
6) You can change the speed of the game in line 537 and 555 of the code, where in inputting any numeric value (in seconds) makes
   the game faster or slower. Currently it's set at 0.01. Reducing the time increases flickering if the number of boxes are huge.
   Feel free to experiment with it.
7) If you want to end the code abruptly then press CTRL+C to do so.   
  
  
