cmake_minimum_required(VERSION 3.22)

project(CppProjectTemplate VERSION 1.0.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# it is common to name a variable in capitalize 
set(LIBRARY_NAME GreetLibrarys)
set(EXECUTABLE_NAME HelloExe)

option(COMPILE_EXECUTABLE "Whether to compile the executable" ON)

add_subdirectory(lib)
if (COMPILE_EXECUTABLE)
    message("With executable compile")
    add_subdirectory(app)
else()
    message("With out executable compile")
endif()

