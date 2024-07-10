cmake_minimum_required(VERSION 3.21)
project(ble_demo)
set(CMAKE_CXX_STANDARD 20)

find_package(simpleble REQUIRED CONFIG)

add_executable(ble_demo main.cpp utils.cpp)

target_link_libraries(ble_demo simpleble::simpleble)

