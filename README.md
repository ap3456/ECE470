# ECE470
Final Project Update 2

Aniket Patel (apate313)
Ashwin Mukund (amukund2)
Anthony Chemaly (chemaly2)
Christopher Kang (cskang2)

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
    
    
    
    
    
