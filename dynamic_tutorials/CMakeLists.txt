cmake_minimum_required(VERSION 3.0.2)
project(dynamic_tutorials)

find_package(catkin REQUIRED COMPONENTS
  dynamic_reconfigure
  roscpp
  rospy
)

generate_dynamic_reconfigure_options(
 cfg/Tutorials.cfg
)

catkin_package(
#  CATKIN_DEPENDS dynamic_reconfigure roscpp rospy
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

