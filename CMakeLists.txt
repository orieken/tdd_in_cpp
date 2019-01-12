cmake_minimum_required(VERSION 3.5)
project(tdd_in_cpp)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES main.cpp ./src/SondexTest.cpp)
add_executable(tdd_in_cpp ${SOURCE_FILES})

include_directories(/usr/local/include)
target_link_libraries(tdd_in_cpp gtest gmock_main)