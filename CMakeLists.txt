cmake_minimum_required(VERSION 3.15)
project(catchExample)

set(CMAKE_CXX_STANDARD 14)

set(MyCatch2Dir /home/rarce/ccom3034)
include_directories(${MyCatch2Dir})
add_executable(catchExample main.cpp ${MyCatch2Dir}/catch_amalgamated.cpp)
