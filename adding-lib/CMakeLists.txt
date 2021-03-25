cmake_minimum_required(VERSION 3.19)
project(adding-library VERSION 1.0.0)

add_library(
    say-hello SHARED
    hello.cpp
    hello.hpp
)

add_executable(addLibrary main.cpp)

target_link_libraries(addLibrary PRIVATE say-hello)