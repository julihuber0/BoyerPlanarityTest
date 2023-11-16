cmake_minimum_required(VERSION 3.5)
project(BoyerPlanarityTest C)

file(GLOB SOURCES *.c)

add_executable(planarity ${SOURCES})