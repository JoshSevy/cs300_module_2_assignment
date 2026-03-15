cmake_minimum_required(VERSION 4.1)
project(CS_300_module_2_assignment)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_executable(CS_300_module_2_assignment
        CSVparser.cpp
        CSVparser.hpp
        VectorSorting.cpp)

foreach(csv IN ITEMS eBid_Monthly_Sales.csv eBid_Monthly_Sales_Dec_2016.csv)
    configure_file(${CMAKE_SOURCE_DIR}/${csv} ${CMAKE_BINARY_DIR}/${csv} COPYONLY)
endforeach()