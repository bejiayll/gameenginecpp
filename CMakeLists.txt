cmake_minimum_required(VERSION 3.31 FATAL_ERROR)

add_subdirectory(external/glfw)
add_subdirectory(external/glad)

set(ProjName GAMEENGINE)
project(${ProjName})
add_executable(${ProjName} src/main.cpp)

target_link_libraries(${ProjName} glfw)
target_link_libraries(${ProjName} glad)


