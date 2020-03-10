cmake_minimum_required(VERSION 3.0)

project(OpenGLTest)

include_directories(BEFORE ${CMAKE_SOURCE_DIR}/include ${CMAKE_SOURCE_DIR}/include)

add_executable(OpenGLTest src/main.cpp src/glad.c)
target_link_libraries(OpenGLTest ${CMAKE_SOURCE_DIR}/libs/glfw3.lib)