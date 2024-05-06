################################################################################
# Set minimum required version of cmake, project name and compile options
################################################################################
cmake_minimum_required(VERSION 3.5)
project(vispa_description)

################################################################################
# Find ament packages and libraries for ament and system dependencies
################################################################################
find_package(catkin REQUIRED)
find_package(urdf REQUIRED)


install(DIRECTORY launch DESTINATION share/${PROJECT_NAME})
install(DIRECTORY rviz DESTINATION share/${PROJECT_NAME})
install(DIRECTORY urdf DESTINATION share/${PROJECT_NAME})
install(DIRECTORY meshes DESTINATION share/${PROJECT_NAME})

################################################################################
# Macro for ament package
################################################################################
catkin_package()

