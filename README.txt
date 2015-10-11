How to run:
python sdmaze.py filename

Output Interpretation:
First the program will solve the puzzle using first hueristic function, then second and finally third

For each function output will be as follows:
First name of the Heuristic function is displayed.
Then if the goal is found, it will say goal found.
Then print Path cost.
Then it will print the mazes starting with showing 1 on the start position and keep on printing mazes at the intermediate state till the goal state is reached.
Along with the states it will also print the dice orientation.

For e.g.

Consider the following maze:
1 G 
. .

Output will be as follows:

------------------------------------Heuristic Function - Euclidean----------------------------
goal Found
Path Cost: 4
----------------------------------------------------------------------------------

1 G 
. . 

Die Orientation for above step
Position: 0, 0
Facing: 1
North: 2
East: 3


1 G 
2 . 

Die Orientation for above step
Position: 1, 0
Facing: 2
North: 6
East: 3


1 G 
2 4 

Die Orientation for above step
Position: 1, 1
Facing: 4
North: 6
East: 2


1 1 
2 4 

Die Orientation for above step
Position: 0, 1
Facing: 1
North: 4
East: 2

Number of nodes added to frontier queue: 6

Number of nodes visited: 6

Then same thing for other two Heuristic functions.

And if the output is not found, it will print following for all 3 functions.
No soloution
Number of nodes added to the frontier queue
Number of nodes visited