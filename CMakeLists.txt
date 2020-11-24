cmake_minimum_required(VERSION 3.1.0)
project(YAMLCPP)

file(GLOB INCLUDES "include")
file(GLOB_RECURSE SRC_FILES "src/*.cpp")

add_library(YAMLCPP ${SRC_FILES})

target_include_directories(YAMLCPP PRIVATE "${INCLUDES}")
set (YAMLCPP_INCLUDES "${INCLUDES}" PARENT_SCOPE)