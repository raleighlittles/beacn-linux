cmake_minimum_required(VERSION 3.22)
project(beacn_linux_driver DESCRIPTION "TODO")

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_FLAGS "-g -O0 -Wall -Wextra -Wpedantic -Wfatal-errors")

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} usb-1.0)