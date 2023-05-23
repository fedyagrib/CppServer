cmake_minimum_required(VERSION 3.20)

set(CMAKE_CXX_COMPILER "g++" CACHE STRING "C++ compiler" FORCE)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_CXX_STANDARD 17)

project(CppServer)

set(SHARED_COMMON "common")

set(CMAKE_BUILD_TYPE Debug)
set (CMAKE_BINARY_DIR "../../build")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/)

include_directories(common/include)

add_subdirectory(common)
add_subdirectory(runtime_tests)
