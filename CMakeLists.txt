cmake_minimum_required(VERSION 4.2.0)

project(betterfpk LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_SCAN_FOR_MODULES OFF)

if(NOT MSVC)
  add_compile_options(-Wno-multichar)
endif()

add_executable(betterfpk
  main.cpp)

install(TARGETS betterfpk)
