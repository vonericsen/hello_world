#min cmake
cmake_minimum_required(VERSION 2.8)

#name
project(hello)

#set output folder
set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR}/lib)

#include folders
include_directories("${PROJECT_SOURCE_DIR}")

add_executable(hello ${PROJECT_SOURCE_DIR}/src/helloworld.cpp)