cmake_minimum_required(VERSION 3.16)
project(EdikyStudio VERSION 0.1 LANGUAGES CXX)

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE Release CACHE STRING "Build type" FORCE)
endif()

add_executable(ediky_editor src/main.cpp)
set_target_properties(ediky_editor PROPERTIES
  CXX_STANDARD 17
  CXX_STANDARD_REQUIRED YES
  CXX_EXTENSIONS NO
)

message(STATUS "Configuring EdikyStudio (${CMAKE_BUILD_TYPE})")
