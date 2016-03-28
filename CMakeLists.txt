cmake_minimum_required(VERSION 2.8.12)
project(sbpl_catkin)

set(CMAKE_BUILD_TYPE Release)

add_subdirectory(sbpl)

set_target_properties(sbpl PROPERTIES OUTPUT_NAME sbpl_catkin)

catkin_package(INCLUDE_DIRS sbpl/src/include LIBRARIES sbpl)
