#Gazebo House ROS2
# Используемое ПО:

  Ubuntu 22.04.5 
  Gazebo 11
  ROS2 Humble
  Gazebo Ignition 6.16.0

#Install Simulation Package

$ cd ~/catkin_ws/src/
$ git clone -b kinetic-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
$ cd ~/catkin_ws && catkin_make

#Launch Simulation TurtleBot3 World

$ export TURTLEBOT3_MODEL=waffle
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch

#How to visualize Simulation data(RViz)

$ roslaunch turtlebot3_gazebo turtlebot3_gazebo_rviz.launch
