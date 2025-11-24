cmake_minimum_required(VERSION 4.0)
project(opengl_tutorial)

# My OS - Fedora 43 KDE Edition

find_package(glfw3 REQUIRED)
find_package(GLEW REQUIRED)
find_package(OpenGL REQUIRED)

set(CMAKE_CXX_STANDARD 20)

add_executable(opengl_tutorial main.cpp)
target_link_libraries(opengl_tutorial glfw GLEW::GLEW OpenGL::GL)
