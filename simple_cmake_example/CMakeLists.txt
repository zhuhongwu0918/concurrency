cmake_minimum_required(VERSION 3.5)
project(SimpleCmakeExample)


add_subdirectory(src)
add_subdirectory(include)

option(BUILD_EXAMPLE "Whether build or not example" ON)

if(BUILD_EXAMPLE)
message(STATUS "Build example...")
    add_subdirectory(example)
endif()
