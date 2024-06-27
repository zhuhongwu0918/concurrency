cmake_minimum_required(VERSION 3.15)
project(Concurrency)

add_subdirectory(thirdparty)
add_subdirectory(include)

option(BUILD_TESTS "Build tests..." ON)
option(BUILD_EXAMPLES "Build examples..." ON)

if(BUILD_TESTS)
    message(STATUS "Building tests...")
    add_subdirectory(tests)
endif()

if(BUILD_EXAMPLES)
    message(STATUS "Building tests...")
    add_subdirectory(examples)
endif()