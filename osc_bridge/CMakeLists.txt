cmake_minimum_required(VERSION 2.4.6)
project(osc_bridge)

find_package(catkin REQUIRED COMPONENTS rospy)


catkin_python_setup()

catkin_package()

catkin_install_python(
  PROGRAMS nodes/osc_bridge.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
