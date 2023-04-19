cmake_minimum_required(VERSION 3.22)

project(CppProjectTemplate VERSION 1.0.0 LANGUAGES C CXX)

add_library(GreetLibrarys STATIC greet_lib.cpp)

add_executable(HelloExe main.cpp)

target_link_libraries(HelloExe PUBLIC GreetLibrarys)




