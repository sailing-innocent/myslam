cmake_minimum_required(VERSION 3.10)

project(HelloSLAM)

add_library(hello_shared SHARED libHelloSLAM.cpp)

# add_executable(helloSLAM helloSLAM.cpp)

add_executable(useHello useHello.cpp)
target_link_libraries(useHello hello_shared)
