# Learning how CMake works

1. Set up github repository for documenting your learning process
2. Create README so that you understand what file is for what
3. Create CMakeLists.txt
> touch CMakeLists.txt --> cmake_minimum_required(VERSION #), project(PROJECTNAME VERSION #)
4. Create build directory
> mkdir build
> cd build
5. Run cmake from *build*
> cmake ../
6. Create executable in CMakeLists.txt
> add_executable(projectname main.cpp)
7. Create main.cpp in main directory
> cd ..
> touch main.cpp
8. Build main.cpp
> cd build
> cmake --build .
9. Run projectname.exe
> ./projectname
