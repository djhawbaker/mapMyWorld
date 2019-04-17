# Map My World
Robo Nano Degree: SLAM project

Using the robot and world from previous projects this one adds SLAM mapping to map an unknown environment.

Instructions to run the project will be updated as it gets completed. These are the instructions from the localization project.

To run, setup two terminals
1. cd catkin_ws
2. catkin_make
3. source devel/setup.bash

Run in separate terminals 
1. roslaunch my_robot world.launch 
2. roslaunch my_robot amcl.launch

Then do one of the following
1. Set a 2D Nav Goal in RViz
2. Setup another terminal and run (This option requires the teleop package as well)
  - rosrun teleop_twist_keyboard teleop_twist_keyboard.py  

The Robot will map it's environment and localize itself within that map by driving around and using SLAM.
