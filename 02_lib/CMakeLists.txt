cmake_minimum_required(VERSION 3.0)
project(02_lib)

set(EXE lib_test)

add_library(hello SHARED hello.cpp hello.h)
add_executable(${EXE} main.cpp)

target_link_libraries(${EXE} hello)
