# Learning how CMake works

## Adding a library

1. Create header file
> touch file.hpp
>> namespace file
>> void function-name();
2. Create header source code
> touch file.cpp
> void function-name() {code}
3. Add header file path in add_executable
> add_executable(target main.cpp header.cpp)
4. Create *build* directory + build using cmake
> mkdir build
> cd build
> cmake ..

## Adding a library (1)

...
- Modify CMakeLists.txt
> add_library(library-name header.cpp header.hpp)
> target_link_library(executable PRIVATE library-name)
