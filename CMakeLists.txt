cmake_minimum_required(VERSION 2.6)

project(linenoise)

include_directories(${linenoise_SOURCE_DIR})

add_library(linenoise linenoise.c)

link_directories(${linenoise_BINARY_DIR})

add_executable(example example.c)
target_link_libraries(example linenoise)

