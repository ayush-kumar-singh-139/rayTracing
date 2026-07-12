cmake_minimum_required(VERSION 3.10)
project(MyMultiFolderProject)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 1. Specify paths to the .cpp files inside the 'src' folder
add_executable(run
    src/main.cpp 
)

# 2. Tell CMake where to look for .h files
target_include_directories(run PRIVATE include)