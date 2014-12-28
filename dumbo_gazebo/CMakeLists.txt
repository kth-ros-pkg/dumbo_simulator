cmake_minimum_required(VERSION 2.8.3)
project(dumbo_gazebo)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS gazebo_ros)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES test
#  CATKIN_DEPENDS dumbo_description
#  DEPENDS system_lib
)


install(FILES
  ${CMAKE_CURRENT_SOURCE_DIR}/launch/dumbo_robotiq_world.launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)