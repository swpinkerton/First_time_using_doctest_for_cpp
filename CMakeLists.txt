cmake_minimum_required(VERSION 3.24)
# Prepare doctest for other targets to use
find_package(doctest REQUIRED)
include(doctest)
project(testtest)

set(CMAKE_CXX_STANDARD 17)

add_executable(testtest testing.cpp)
doctest_discover_tests(testtest)
