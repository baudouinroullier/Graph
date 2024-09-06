cmake_minimum_required(VERSION 3.17)

project(Graph CXX)

## Build static library

set(LIB_NAME "graph")
add_library(${LIB_NAME}
    include/graph/Graph.h
    include/graph/algo.h
)
set_property(TARGET ${LIB_NAME} PROPERTY CXX_STANDARD 20)
set_target_properties(${LIB_NAME} PROPERTIES LINKER_LANGUAGE CXX)

target_include_directories(${LIB_NAME} PRIVATE "include/graph")
