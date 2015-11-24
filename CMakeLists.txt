cmake_minimum_required(VERSION 2.6)
project(lib3d)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -g -std=c++11")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -g")

set(SOURCES
	source/main.cpp
)

add_executable(${PROJECT_NAME} ${SOURCES})

target_link_libraries(${PROJECT_NAME} SDL2 GL GLEW)
