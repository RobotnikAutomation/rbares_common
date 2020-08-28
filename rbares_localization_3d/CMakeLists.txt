cmake_minimum_required(VERSION 2.8.3)
project(rbares_localization_3d)

find_package(catkin REQUIRED COMPONENTS
)

###################################
## catkin specific configuration ##
###################################

catkin_package(
  CATKIN_DEPENDS
)

###########
## Build ##
###########

install(
  DIRECTORY launch maps config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
