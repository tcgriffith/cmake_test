# Specify the minimum version for CMake

cmake_minimum_required(VERSION 2.8)

# Project's name

project(test)

set(CMAKE_BINARY_DIR ${CMAKE_HOME_DIRECTORY}/bin)
set(CMAKE_SOURCE_DIR ${CMAKE_HOME_DIRECTORY}/src)
set(CMAKE_CXX_STANDARD 11)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})

add_executable(tester ${CMAKE_SOURCE_DIR}/main.cc ${CMAKE_SOURCE_DIR}/ns.cc ${CMAKE_SOURCE_DIR}/tmp.cc )

