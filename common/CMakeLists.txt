cmake_minimum_required(VERSION 3.20)

find_package (Threads)

project(${SHARED_COMMON} CXX)

add_library ( 
    ${PROJECT_NAME} STATIC
    sources/test.cpp
)
