cmake_minimum_required(VERSION 3.17)

set(LIB_NAME "Graph")
project(${LIB_NAME} CXX)

add_library(${LIB_NAME}
    include/Graph/Graph.h
    include/Graph/algo.h
)
set_target_properties(${LIB_NAME} PROPERTIES CXX_STANDARD 20 LINKER_LANGUAGE CXX)

target_include_directories(${LIB_NAME} PRIVATE "include/Graph")
