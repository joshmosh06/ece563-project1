cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "-Wall -Werror")
project(ece563-project1)

add_library(src ../sim_pipe.h ../sim_pipe.cc ../sim_pipe_fp.cc ../sim_pipe_fp.h lib/sp_register.h lib/sp_register.cpp)

add_subdirectory(testcases)
add_subdirectory(asm)
add_subdirectory(lib)