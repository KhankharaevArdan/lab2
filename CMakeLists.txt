cmake_minimum_required(VERSION 3.16)
project(Integral)

set(CMAKE_CXX_STANDARD 14)
add_compile_options(-pthread)
add_executable(Integral main.cpp)

find_package(Threads)
target_link_libraries(Integral PRIVATE Threads::Threads)