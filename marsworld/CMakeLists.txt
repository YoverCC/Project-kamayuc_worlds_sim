cmake_minimum_required(VERSION 3.0.2)
project(marsworld)

find_package(catkin REQUIRED COMPONENTS
  gazebo_ros
)

catkin_package()

install(DIRECTORY models/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/models
)

install(DIRECTORY worlds/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/worlds
)