cmake_minimum_required(VERSION 3.5)
project(BoyerPlanarityTest C)

set(CMAKE_C_FLAGS_DEBUG "-O0 -g -Wall")
set(CMAKE_C_FLAGS_RELEASE "-O3 -g -DNDEBUG -march=native -mtune=native")
message("CMAKE_BUILD_TYPE is ${CMAKE_BUILD_TYPE}")
message("CMAKE_C_FLAGS_DEBUG is ${CMAKE_CXX_FLAGS_DEBUG}")
message("CMAKE_C_FLAGS_RELEASE is ${CMAKE_CXX_FLAGS_RELEASE}")
message("CMAKE_C_FLAGS is ${CMAKE_CXX_FLAGS}")

file(GLOB SOURCES *.c)

add_executable(planarity ${SOURCES})