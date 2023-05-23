cmake_minimum_required(VERSION 3.20)

project(tests CXX)

find_package(Threads REQUIRED)

add_executable ( 
    ${PROJECT_NAME}
    main.cpp
)

target_link_libraries(${PROJECT_NAME} ${SHARED_COMMON})
