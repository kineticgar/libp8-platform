cmake_minimum_required(VERSION 2.8.3)
project(libplatform)

# You cloned with git clone --recursive, right?
add_subdirectory(lib/platform)

find_package(catkin REQUIRED)
catkin_package(
  INCLUDE_DIRS lib/platform/src
  LIBRARIES platform
)

