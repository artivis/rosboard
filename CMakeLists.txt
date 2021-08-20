cmake_minimum_required(VERSION 2.8.3)
project(rosboard)

find_package(catkin REQUIRED COMPONENTS)

catkin_python_setup()
catkin_package()

catkin_install_python(PROGRAMS
  nodes/rosboard_node
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
