cmake_minimum_required(VERSION 3.0)

project(OpenGLTest)

include_directories(BEFORE ${CMAKE_SOURCE_DIR}/include)

add_library(glad libs/glad/glad.c)
include_directories(${CMAKE_SOURCE_DIR}/libs)

add_executable(OpenGLTest src/main.cpp)
target_link_libraries(OpenGLTest glad ${CMAKE_SOURCE_DIR}/libs/glfw3.lib)
