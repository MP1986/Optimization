------------------------
Running this Application
------------------------

Download the GitHub repository and open index.html in the main directory
and pizza.html in the views directory to view the two pages optimized
for this project.  Alternately, you may visit the URL 
www.cowsaysgethyphy.com.

----------------------------------------------------------------
Optimizations made to index.html to achieve PageSpeed score > 90
----------------------------------------------------------------

Linked CSS and JS files were inlined into the code and placed at the
bottom of the file to eliminate render blocking.

Inlinted font styling and directly linked it from the URL the font
is pulled from.

Code was minified.

--------------------------------------------------------
Optimizations made to views/js/main.js to achieve 60 FPS
--------------------------------------------------------

In the updatePositions() function on line 519, the phase calculation 
results were placed into an array, which is then called by a for loop, 
so the calculation will not be performed each iteration.

In the for loop on line 568, the max value of i was converted to the
value of the screen height multiplied by var row times var cols.

All querySelector tags were converted to getElementById or 
getElementsByClassName.

Calculations and variable declarations nested inside for loops were 
moved into local variables that are then called inside the for loop.

Code was minified.