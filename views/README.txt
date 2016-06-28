------------------------
Running this Application
------------------------

Download the GitHub repository and open index.html in the main directory.
Alternately, you may visit the URL www.cowsaysgethyphy.com.

--------------------------------------
Optimizations made to views/js/main.js
--------------------------------------

In the updatePositions() function on line 519, the phase calculation 
results were placed into an array, which is then called by a for loop, 
so the calculation will not be performed each iteration.

In the for loop on line 568, the max value of i was reduced to 40,
as 200 is far more pizzas than can fit onscreen at a time.

main.js was minified.