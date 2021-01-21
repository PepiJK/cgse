cmake_minimum_required(VERSION 3.17)
project(cgse)

set(CMAKE_CXX_STANDARD 20)

add_executable(cgse main.cpp shader/shader.h)

target_sources(cgse PRIVATE lib/glad/glad.c)
target_link_libraries(cgse glfw)
target_link_libraries(cgse GL)
target_link_libraries(cgse X11)
target_link_libraries(cgse pthread)
target_link_libraries(cgse Xrandr)
target_link_libraries(cgse Xi)
target_link_libraries(cgse dl)
