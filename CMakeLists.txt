cmake_minimum_required(VERSION 3.13)

project(Hello)

enable_testing()

add_library(${PROJECT_NAME} hello.cpp hello.h)
target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(test)