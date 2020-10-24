# SLAM_RTABMap_usingROS
ROS Project to practice SLAM using RTBMap package in a custom world

### 3D Point Cloud View:
![Point Cloud](https://github.com/dhruvtya/SLAM_RTABMap_usingROS/blob/main/Point%20Cloud.jpg)

### Finding Common Features & Loop Closure:
<img src="https://github.com/dhruvtya/SLAM_RTABMap_usingROS/blob/main/Screenshot%203.JPG">

<img src="https://github.com/dhruvtya/SLAM_RTABMap_usingROS/blob/main/Screenshot%206.JPG">

### Built on:
ROS Kinetic & Ubuntu 16.04

## Steps to Implement:
1. Create a Catkin Workspace and clone the repo and store it as 'my_robot' package in the 'src' folder.
2. Clone the following ROS Package into the src folder : http://wiki.ros.org/rtabmap_ros
3. Clone the teleop package into the src folder : https://github.com/ros-teleop/teleop_twist_keyboard
4. Change back to the catkin workspace folder and execute ```catkin_make```
5. ```source devel/setup.bash```
6. ```roslaunch my_robot world.launch```
7. In a new terminal : ```rosrun teleop_twist_keyboard teleop_twist_keyboard.py```
8. In a new terminal : ```roslaunch my_robot mapping.launch```
9. Command the robot around using the teleop terminal. When done, close all the terminals.
10. The map file, 'rtabmap.db', will be created in a hidden folder '~/.ros'

### View the map file: 
In a new terminal execute : ```rtabmap-databaseViewer ~/.ros/rtabmap.db```
(Could not provide the rtabmap.db file I generated due to file size limitations. Screenshot is provided above)
