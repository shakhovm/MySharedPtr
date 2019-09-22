cmake_minimum_required(VERSION 3.14)
project(shared_ptr)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(googletest-master/googletest)
include_directories(googletest-master/googletest/include)

add_executable(shared_ptr main.cpp mySharedPtr.h)

target_link_libraries(shared_ptr gtest gtest_main)