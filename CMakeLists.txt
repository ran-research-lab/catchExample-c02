cmake_minimum_required(VERSION 3.15)
project(catchExample)

set(CMAKE_CXX_STANDARD 14)

set(CATCH2DIR /home/rarce/ccom3034)

IF(EXISTS ${CATCH2DIR})   
  include_directories(${CATCH2DIR})
  add_executable(catchExample main.cpp ${CATCH2DIR}/catch_amalgamated.cpp)
else()
  add_executable(catchExample main.cpp catch_amalgamated.cpp)
endif()
