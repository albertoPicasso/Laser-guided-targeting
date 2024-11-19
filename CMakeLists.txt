cmake_minimum_required(VERSION 3.0)
project(Laser-guided-targeting)

# Find OpenCV package
find_package(OpenCV REQUIRED)

# Include directories from OpenCV
include_directories(${OpenCV_INCLUDE_DIRS})

# Create an executable
add_executable(Laser-Tracker main.cpp)

# Link OpenCV libraries
target_link_libraries(Laser-Tracker ${OpenCV_LIBS})
