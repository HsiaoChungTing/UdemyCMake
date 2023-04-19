add_library(${LIBRARY_NAME} STATIC src/greet_lib.cpp)
target_include_directories(${LIBRARY_NAME} PUBLIC "./include")

