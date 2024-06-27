project(SimpleCmakeExample)


add_library(simplecmake SHARED  printhello.cpp)

# message(STATUS "ZHHW: ${CMAKE_CURRENT_SOURCE_DIR}/../include")

target_include_directories(simplecmake
PUBLIC
${CMAKE_CURRENT_SOURCE_DIR}/../include
)