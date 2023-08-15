cmake_minimum_required(VERSION 3.22.0)
project(MyProject)

add_subdirectory(../Catch2 Catch2-build)
add_executable(MyProjectTest test-main.cpp)
target_link_libraries(MyProjectTest PRIVATE Catch2::Catch2)