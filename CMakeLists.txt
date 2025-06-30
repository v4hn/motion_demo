cmake_minimum_required(VERSION 3.0.2)
project(motion_demo)

find_package(catkin REQUIRED COMPONENTS
  dynamic_reconfigure
  rospy
  moveit_commander
)

generate_dynamic_reconfigure_options(
  cfg/Velocity.cfg
)

catkin_package()
