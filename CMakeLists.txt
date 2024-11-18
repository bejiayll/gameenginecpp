cmake_minimum_required(VERSION 3.31)

add_subdirectory(external/glfw)

set(ProjName GAMEENGINE)
project(${ProjName})
add_executable(${ProjName} src/main.cpp)

target_link_libraries(${ProjName} glfw)
