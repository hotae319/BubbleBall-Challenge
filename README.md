# Bubble ball code Description

## Structure
* We have 2 python scripts. (One is for parsing and running the simulation / The other one is for handling the log file)
* `parsing_movableobjects_levels.py` : It has 2 functions (parsing_objects, run_simulation)
* `log2matrix.py` : It has 1 function (logging_trajectory)

## Prerequisite
* Required to have **automate.json, (level).json, movableObjects.json, bb.log** in the same folder as two python scripts.
* If you change the import line, you can make a directory and put those files into that.
* Of course, you should have a bubble-ball game file. (You need to obtain License and linux-execution file from Naygames)
* If you wanna change the level, you have to import this module and use the function with argument(level)  

## How to use 
* Ex) level 2 (It is already selected in __main__.)
1. Locate the requires files in the same folder(You can put this two python scripts into the bubble ball game directory)
2. run parsing_movableobjects_levels.py
3. It will ask you to enter the initial configuration you want for each ID. 
ex) Input the configuration [x,y,r] list of the metal block on [0, 8, 150, 25, 0] with "AO6G" ID. You should enter the numbers by space: 
4. You can enter like 210 235 0
5. It is gonna ask you about others iteratively
6. When you complete entering all values, bubble-ball game will start with the initial configuration you enter and save the log
7. You can run log2matrix.py in order to analyze the log file 
8. It returns the arrays or lists which are already categorized.
9. We can use it