# MD
Well... you and I just wanna know how this thing works, or what doesn´t work (yet :smile: ) in the shortest time ....  

## [src](https://github.com/marcvty98/MD/tree/main/src)
1. Here you can find two directories:
  - [mobile_robot_navigation](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation)
  - [ydlidar_ros_driver](https://github.com/marcvty98/MD/tree/main/src/ydlidar_ros_driver)
 
2. These needs to be moved in your ROS workspace (copy or cut). 

3. Compile your ROS workspace
```
ctrl+alt+t
cd "your_ROS_workspace"
catkin_make
```

### [mobile_robot_autonomous_navigation](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation)

#### [arduino_code](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/arduino_code)
Here there are only two directories with one file each one, the arduino code for each control wheel. Both codes are same, i2c direction is the unique difference between. 

#### [config](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/config)
The specific ROS settings to do SLAM:
  - local and global map settings
  - velocity, acceleration and jerk limits
  - joint limits
  - mapping configurations
  - path planning
  - rviz profilesand
 
 Are here.

#### [launch](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/launch) 
To do SLAM ROS tasks:
  - Checking the URDF file
  - Cheking ans testing robot's controllers
  - Mapping settings
  - Autonomous navigations settings

#### [maps](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/maps)
After explorations task, all maps will be saved there. 

#### [scripts](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/scripts)
Personal Python scripts for navigation can be created, like:
  - Sequential goals
  - Petitions by terminal to arrive somewhre
  - etc

#### [stl](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/stl)
Personal designs, crated in CAD/CAM tools, like:
  - robot cases
  - wheels
  - sesnors cases
  - robotic arms (or his parts)
  - mechanisms (like exoskeletons)
  -etc

These will be here with a .stl or .STL extention. 

#### [urdf](https://github.com/marcvty98/MD/tree/main/src/mobile_robot_autonomous_navigation/urdf)
Robot setup can be constructed with one or some files with .urdf extension.

### ydlidar_ros_driver
To use a Lidar with ros, you need ROS settings too. Well, everything about how lidar sensor works are here.

The current project is completely configured with and no necessary do changes in this directory. But, if you want to know more about the YDLIDAR X4 sensor, you can see his GitHub repository [here](https://github.com/YDLIDAR/ydlidar_ros).

## 3D Printing stl files
You will see the following directories and files within: 
  - Carcasa para KY040
    - box.STL
    - tapa.STL
  - Engranajes
    - engrj.STL
    - pinon.STL
  - Nivelador
    - eje.STL
  - Ranura
    - ranura2.STL
 
 These files are ready to be printed. 

## Design
The project design was divided in two parts:
1. Diseño para el Sistema de Locomoción: Every part for the robot can do moves (rotations and rotations).
2. Diseño para el Sistema de Conteo: Every part part for the robot can do Odometry.

## Electrical Diagrams-
