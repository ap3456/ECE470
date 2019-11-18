# ECE470
Aniket Patel (apate313)
Ashwin Mukund (amukund2)
Anthony Chemaly (chemaly2)
Christopher Kang (cskang2)


Final Project Update 4

This code is designed for a UR3 robot to be able to stack upto 9 cups in V-rep simulation using the BaxterVaccumCup. The robot now creates a Pyramid structured stack instead of a 2D triangular stack.
We will be using the default values for vel, accel, jerk, currentvelocity and current acceleration. Joints of the robot uses radians as an input, thus d2r variable was created in order to make the conversion. We use the default maxvel, maxaccel,  maxjerk, and target velocity values. We have defined a new variable named number to assign the number of cups that the robot needs to stack. Based on the value of the number variable, the programs picks the if case that is relevant to the problem.  
Each case contains the steps to stack the assigned number of cups as follows: 
    1) Set the starting position. 
    2) Move to the starting position. 
    3) Set the position on top of the cup (that needs to be stacked) in such a way that the gripper is touching the cup. This is to ensure that the gripper can pick up the cup. 
    4) Move to the new location. 
    5) Turn the suction on.
    6) Set a new position. This is the position where you want to place the cup.
    7) Move to the new position. 
    8) Turn the suction off.
    Now repeat steps 3-8 for all of the remaining cups that needs to be stacked. Updates the positions in step 3 and 6 to reflect the new locations of the cups.
    9) Assign the base position.
    10) Move to the base position.
    


Final Project Update 3

This code is designed for a UR3 robot to be able to stack three cups in V-rep simulation using the BaxterVaccumCup. 
We will be using the default values for vel, accel, jerk, currentvelocity and current acceleration. Joints of the robot uses radians as an input, thus d2r variable was created in order to make the conversion. We use the default maxvel, maxaccel,  maxjerk, and target velocity values.
The steps to stack three cups are as follow: 
    1) Set the starting position. 
    2) Move to the starting position. 
    3) Set the position on top of the first cup in such a way that the gripper is touching the cup. This is to ensure that the gripper can pick up the cup. 
    4) Move to the new location. 
    5) Turn the suction on
    6) Set a new position. This is the position where you want to drop the first cup.
    7) Move to the new position. 
    8) Turn the suction off.  
    9) Set the position on top of the second cup in such a way that the gripper is touching the cup. This is to ensure that the gripper can pick up the cup. 
    10) Move to the new location. 
    11) Turn the suction on
    12) Set a new position. This position is right next to the first cup in such a way that the rim of the two cups are touching.
    13) Move to the new position. 
    14) Turn the suction off. 
    15) Set the position on top of the third cup in such a way that the gripper is touching the cup. This is to ensure that the gripper can pick up the cup. 
    16) Move to the new location. 
    17) Turn the suction on
    18) Set a new position. This position is centered on top of the first two cups' location. This is to allow for the stacking of the third cup on top of the first two cups. 
    19) Move to the new position. 
    20) Turn the suction off.
    21) Set and move to the end location. This is just out of the way of our tower of cup formation. 


Final Project Update 2

This code is designed for a UR3 robot to pick up and move a lighly dense concerete block in the V-rep simulation. 
The UR3 robot is a 6 joint arm basaed robot that is stationary. The joints are controlled through precise angular movements. We are using the BaxterVaccumCup to pick up the object using its suction capability. 

We will be using the default values for vel, accel, jerk, currentvelocity and current acceleration. Joints of the robot uses radians as an input, thus d2r variable was created in order to make the conversion. We use the default maxvel, maxaccel,  maxjerk, and target velocity values. 
The steps to picking up and moving the object are as follows: 
    1) Set the starting position. 
    2) Move to the starting position. 
    3) Set the position on top of the block in such a way that the gripper is touching the block. This is to ensure that the gripper can pick up the block. 
    4) Move to the new location. 
    5) Turn the suction on
    6) Set a new position. This is the position where you want to drop the block.
    7) Move to the new position. 
    8) Turn the suction off. 
