# Installing-arm-package-on-ROS
Installing arm package on Robotics Operating System ( ROS ) and Controlling the arm motors in simulation 
# Steps
run this instruction inside your workspace:

$ cd simulation_ws
$ cd src/
$ git clone https://github.com/smart-methods/arduino_robot_arm.git
$ cd ..
$ ls
$ catkin_make

# for melodic distro

$ sudo apt-get install ros-melodic-moveit
$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

# Controlling the robot arm by joint_state_publisher

$ roslaunch robot_arm_pkg check_motors.launch

# Simulation
( Run the following instructions to use gazebo )

$ roslaunch robot_arm_pkg check_motors.launch
$ roslaunch robot_arm_pkg check_motors_gazebo.launch
$ rosrun robot_arm_pkg joint_states_to_gazebo.py

# Controlling the robot arm by Moveit and kinematics

$ roslaunch moveit_pkg demo.launch

# Simulation

$ roslaunch moveit_pkg demo_gazebo.launch

# Robot initial positions





Randomize


