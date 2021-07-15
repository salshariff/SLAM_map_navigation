# SLAM_map_navigation

 ## Using the SLAM map to start navigation
 
   ### Launch Simulation World
 
 ```
$ export TURTLEBOT3_MODEL=waffle_pi
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
```

   ### Run Navigation Node

in new terminal 

```
$ export TURTLEBOT3_MODEL=waffle_pi
$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
```
   ### Estimate Initial Pose
 
 Before turning on the navigation
 
 - click the [2D Pose Estimate] in the RViz menu
 
 - Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.
 
 - Launch keyboard teleoperation node to precisely locate the robot on the map.
 
 ``` $ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch ```
 
   ### Set Navigation Goal

- click the [2D Nav goal] in RViz menu.

- Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing.

<img width="1370" alt="Screen Shot 1442-12-05 at 6 16 36 AM" src="https://user-images.githubusercontent.com/85907057/125723728-ec3b3a2e-a709-4582-808d-2c50895fe2da.png">

