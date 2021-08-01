# Grid-System
# columns and rows for main container and column and row for single element.
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
 
            grid-column-start: 1;
            grid-column-end: 3; 

            shortcut of start and end .
            grid-column: 1/3;
             or  
            grid-column: 1/-1

            That means. This content will start from first column and end to the 3 column. which is last column.

            Third syntax is 
            grid-column : 1/ span 2;
            grid-column : start from 1 column / and span 2;
            
10. Making 12 grid :

            grid-template-columns: repeat(12, 1fr);

11. Maintaining height of rows. At first you have to give a height of a container :

            grid-template-rows: 50px 1fr 1fr 50px;
            height: 100vh;

12. Using grid-template-areas we can visually decorate our layout.

13. Using auto-fit and minmax function is a best way for responsiveness. 
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            grid-template-rows: repeat(3, 1fr);