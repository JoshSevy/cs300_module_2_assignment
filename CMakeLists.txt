cmake_minimum_required(VERSION 4.1)
project(CS_300_module_2_assignment)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_executable(CS_300_module_2_assignment
        CSVparser.cpp
        CSVparser.hpp
        VectorSorting.cpp)
