cmake_minimum_required(VERSION 3.15)
project(opencv)

set(CMAKE_CXX_STANDARD 17)
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(opencv_example img_gscale.cpp)
target_link_libraries(opencv_example ${OpenCV_LIBS})
