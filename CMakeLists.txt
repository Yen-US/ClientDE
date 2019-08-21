cmake_minimum_required(VERSION 3.14)
project(ClientDE)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(SOURCE_FILES main.cpp)
find_package(Qt5Sql REQUIRED)

set(CMAKE_CXX_STANDARD 14)

add_executable(ClientDE main.cpp)
target_link_libraries(ClientDE Qt5::Widgets Qt5::Sql)