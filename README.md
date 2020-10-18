# Robotman
Humanoid robot for security and guidance!

Robotman is a robot that combines qualities for interaction with humans, and security patrolling services. The robot is able to perform security patrols during the night while functioning as a guide during the day. 

Video of the simulation of the robot:

 * https://youtu.be/itvLRondz2I
 
<img src="https://github.com/robotswithros/robotman/robotman_mall.jpeg" width="200" height="400">
 
 # Tutorial
 
 Download the robot in your ROS-workspace, I call my ros_ws. If you don't have one, you can created with the following steps:
 
 ```
 mkdir -p ~/ros_ws/src
 cd ~/ros_ws/
 catkin_make
 source devel/setup.bash
 cd src/
 git clone https://github.com/robotswithros/robotman.git
 cd ..
 catkin_make
 ```
 
 This simulation was develop for ROS Melodic and Ubuntu 18.04. Use the follow comand to spawn the robot in Gazebo:
 
 ```
 roslaunch robotman_gazebo spawn_robot.launch
 ```
 
 ![Robotman_Gazebo](Robotman_gazebo.png)
 
 There is a node you could use to change the image show in the touch screen of the robot:
 
 ```
 rosrun robotman_gazebo display_screen.launch
 ```
 
 There is a node to teleoperate the base of the robot:
 
 ```
 rosrun robotman_gazebo robotman_teleop.launch
 ```
 
