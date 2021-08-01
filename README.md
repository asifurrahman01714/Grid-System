# Grid-System

1. At first you have to style as display: grid to design your layout according to grid system.
2. Add grid-template-columns and rows. where the pixel is the width for columns and height for rows
3. We can add grid row and column gap by grid-row-gap and grid-column-gap
4. For same gap in row and column write grid-gap only
5. For responsive pixel is disgusting. So use fraction unit like-
            grid-template-columns: 1fr 2fr;  
            grid-template-rows: 1fr 2fr;

6. use one line codding for both columns and rows. like-

            grid-template: 1fr 2fr / 1fr 1fr 1fr;
            Which is actually-
            grid-template : rows / columns;

7. For same width and height or repeating rows and columns we can short our code by using repeat() function. like- 

            grid-template: repeat(3, 1fr) / repeat(2, 1fr);

8. for giving full width of a special content use grid-column-start and end.

            grid-column-start: 1;
            grid-column-end: 3;

9. Grid column start and end shortcut :
 
             /* grid-column-start: 1;
            grid-column-end: 3; */

            /* shortcut of start and end . */
            /* grid-column: 1/3;
             or  */
            grid-column: 1/-1