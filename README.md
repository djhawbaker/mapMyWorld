# Map My World
Robo Nano Degree: SLAM project

Using the robot and world from previous projects this one adds SLAM mapping to map an unknown environment.
Includes the RTABMAP ROS package found here: http://wiki.ros.org/rtabmap_ros

### To run, setup three terminals and run the following in each
1. cd catkin_ws
2. catkin_make
3. source devel/setup.bash

## Mapping
Run in separate terminals 
1. roslaunch my_robot world.launch 
2. roslaunch my_robot teleop.launch
3. roslaunch my_robot mapping.launch

Drive the robot around the environment with the teleop terminal until the robot has gone through the full environment and has found a minimum of 3 loop closures. 

The database will be located in 
``` 
/root/.ros/
```

Use rtabmap-databaseViewer to analyze the map data
```
rtabmap-databaseViewer /root/.ros/rtabmap.db
```

## Localization
Run in separate terminals 
1. roslaunch my_robot world.launch 
2. roslaunch my_robot teleop.launch
3. roslaunch my_robot localization.launch

