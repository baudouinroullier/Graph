cmake_minimum_required(VERSION 3.17)

set(LIB_NAME "Graph")
project(${LIB_NAME} CXX)

## Build static library

add_library(${LIB_NAME}
    include/Graph/Graph.h
    include/Graph/algo.h
)
set_property(TARGET ${LIB_NAME} PROPERTY CXX_STANDARD 20)
set_target_properties(${LIB_NAME} PROPERTIES LINKER_LANGUAGE CXX)

target_include_directories(${LIB_NAME} PRIVATE "include/Graph")
