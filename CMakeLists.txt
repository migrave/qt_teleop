cmake_minimum_required(VERSION 2.8.3)
project(qt_teleop)

find_package(catkin REQUIRED COMPONENTS
  roslint
  rospy
  roslaunch
  joy
  sensor_msgs
)

roslint_python()
catkin_python_setup()

catkin_package(
  CATKIN_DEPENDS
    rospy
    roslaunch
    joy
    sensor_msgs
    std_msgs
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

install(PROGRAMS
  ros/scripts/joy
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}/scripts
)

install(DIRECTORY ros/launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)
