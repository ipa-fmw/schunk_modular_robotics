cmake_minimum_required(VERSION 2.8.3)
project(schunk_sdhx)

find_package(catkin REQUIRED COMPONENTS)

catkin_package()

install(PROGRAMS src/sdhx_node.py src/recover_gripper.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}/src
)
