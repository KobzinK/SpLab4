cmake_minimum_required(VERSION 3.10)

project(MyCalculator)

set(CMAKE_CXX_STANDARD 11)

add_library(calculator calculator.cpp calculator.h)

add_executable(calculator_app main.cpp)

target_link_libraries(calculator_app calculator)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
