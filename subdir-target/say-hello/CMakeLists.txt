add_library(
    say_hello
    src/sayHello/hello.cpp
    src/sayHello/hello.hpp
)

target_include_directories(say_hello PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/src")