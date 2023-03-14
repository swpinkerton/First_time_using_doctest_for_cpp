cmake_minimum_required(VERSION 3.24)
project(testtest)

set(CMAKE_CXX_STANDARD 17)

add_executable(testtest main.cpp testing.cpp)
doctest_discover_tests(testtest)
