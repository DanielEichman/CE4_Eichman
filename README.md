CE4_Eichman
===========

##Program A Code Listings 
![Code File](https://github.com/DanielEichman/CE4_Eichman/blob/master/SimpleMemoryManipulation.psm)

![Code JPG](https://raw.githubusercontent.com/DanielEichman/CE4_Eichman/master/SMM_Code.JPG)

This code stores three values (9, 8, and B) in three RAM locations (B0, C4, and CB). The loop at the end of the code is so that program doesn't crash when it reaches the end of the instruction set. I also was able to complete the code by the target program end of 11. 
####Results
At the end of the program the value's in the RAM were correct. 9 was in B0, 8 was in C4, and B was in CB.
##Program B Code Listings 

![Code File](https://github.com/DanielEichman/CE4_Eichman/blob/master/Math.psm)

![Code JPG](https://raw.githubusercontent.com/DanielEichman/CE4_Eichman/master/Math_Code.JPG)

This code takes the value at RAM B0 doubles in and subtracts 4. To do this the value was loaded onto the accumulator. Then the value at B0 was added to the accumulator. This essentially doubles it. Now we have to subtract 4, however there is no subtracting function. To do this the 2's complement of 4 needed to be added to the accumulator. The two's complement of 4 is C. Finally the infinite loop is reached so the program will not crash. I also was able to complete the code by the target program end of 0C. 

####Results
At the end of the program the math was done correctly. For and input of 6 output port 3 displayed 8. 4 outputted 4, 8 gave C.


##Program C Code Listings
![Code File](https://github.com/DanielEichman/CE4_Eichman/blob/master/Loops.psm)

![Code JPG](https://raw.githubusercontent.com/DanielEichman/CE4_Eichman/master/Loop_Code.JPG)

This program takes an input from input port 3, and then outputs the value on output port 0 and one less on output port 1 and one less again one output port 2. First we load the value into the accumulator. Next we display the value on output port 0. Next we subtract 1 by added the 2's complement of 1 (F) to it. The last addition is so that the next time through the loop it will appear as if it only decreased by 1. Lastly the loop keeps the program running forever. I also was able to complete the code by the target program end of 10.

####Results
At the end of the program the program worked as designed. For an input of 9 the outputs were as followed: (output port 3,output port 2, output port 1) after the first cycle (9,8,7) second cycle (8,7,6) third cycle (7,6,5). This continued forever.
