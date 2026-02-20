cmake_minimum_required(VERSION 3.16)

project(QtTest)

set(CMAKE_CXX_STANDARD 17)

find_package(Qt6 REQUIRED COMPONENTS Widgets)

qt_standard_project_setup()

add_executable(QtTest main.cpp)

target_link_libraries(QtTest PRIVATE Qt6::Widgets)