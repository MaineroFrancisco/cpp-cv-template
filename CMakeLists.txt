cmake_minimum_required(VERSION 3.31)
project(CV_Template CXX)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Find the packages declared in vcpkg.json

find_package(opencv CONFIG REQUIRED)

find_package(opengl REQUIRED)

#
set(SOURCE_FILES src/main.cpp)

#
set(HEADER_FILES)

add_executable(CV_Template ${SOURCE_FILES} ${HEADER_FILES})

target_link_libraries(CV_Template PRIVATE)
