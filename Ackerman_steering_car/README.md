# Ackerman_steering_car

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

## Overview
In this project we worked on the four wheeled car with independent steering joints. The name of the robot package is ‘robot_car’.
URDF file was generated using solidworks and integrated in ROS. Required files for Launching and controlling the robot in Gazebo and Rviz were created.
CAD files have also been included.
## Import 

Import package robot_car to the workspace:

```sh
cd catkin_ws/src
git clone https://github.com/tarunreddyy/Ackerman_steering_car.git
```

## Simulation

For Gazebo simulation run the below command in the terminal:

```sh
roslaunch robot_car robot_car.launch
```

The car is spawned in the custom build gazebo world. To control the car run the below command in the terminal:

```sh
rosrun robot_car teleop_node.py
```

Follow the instructions displayed in the terminal to increase/decrease velocity. 
The car is equipped with a LiDAR, to see the LiDAR scan data in rviz use the below command:

```sh
roslaunch robot_car display.launch
```
Add the RobotModel (Fixed frame: base_link) and for LiDAR data add LidarScan (choose topic) to see the output. Joint_state_publisher_gui is also launched with rviz. 
