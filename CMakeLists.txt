cmake_minimum_required(VERSION 3.22)

project(giza)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_BUILD_TYPE Debug)

# add_subdirectory(external/cpp-linenoise)
set(giza_sources
src/main.cpp)

add_executable(giza ${giza_sources})

target_include_directories(giza PUBLIC include)
target_include_directories(giza PUBLIC external/cpp-linenoise)