<!--![](/images/.jpg?raw=false)-->

# Simultaneous Localization and Mapping (SLAM) 

> In computational geometry and robotics, simultaneous localization and mapping (SLAM) is the computational problem of constructing or updating a map of an unknown environment while simultaneously keeping track of an agent 's location within it.
> 

It is the process of buiilding a map using range sensors (e.g. laser sensors, 3D sensors, ultrasonic sensors) while the robot is moving around and exploring an unknown area.

Sensor Fusion: This process uses filtering techniques like Kalman filters or particle filters.

![](Slam.gif)
---

## Table of Contents
- [Built With](#built-with)
- [Turtlebot3 Slam](#Turtlebot3_Slam-package)
- [Turtlebot3 Gazebo](#Turtlebot3_Gazebo-package)
---

## Built With
The ROS workspace first needs to be initialized
```javascript
mkdir ~/catkin_ws/src/
cd ~/catkin_ws
catkin_init_workspace
```
afterwards, the repository can be cloned or downloaded and unzipped in the corresponding path. The packages can be compiled, and the environment has to be sourced.

```
catkin_make
source devel/setup.bash
```

Next, the robot is started inside the gazebo world, and the visualization program RVIZ is opened.

```
roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
 
```

## turtlebot3_Slam-package

One of The TurtleBot3’s core technology is SLAM, Navigation and Manipulation. Navigation allows the robot to move from one location to a specified destination in a given environment. For this purpose, a map that contains geometry information of furniture, objects, and walls of the given environment is required. The map was created with the distance information obtained by the sensor and the pose information of the robot itself.

## turtlebot3_Gazebo-package

The TurtleBot3’s core technology is SLAM, Navigation and Manipulation, making it suitable for home service robots. The TurtleBot can run SLAM(simultaneous localization and mapping) algorithms to build a map and can drive around your room. 

Gazebo offers the ability to accurately and efficiently simulate populations of robots in complex indoor and outdoor environments. At your fingertips is a robust physics engine, high-quality graphics, and convenient programmatic and graphical interfaces. 

---


