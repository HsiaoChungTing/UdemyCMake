cmake_minimum_required(VERSION 3.22)

project(CppProjectTemplate VERSION 1.0.0 LANGUAGES C CXX)

# lib要比app前面因為app會使用到lib所以要先編譯lib app才能直接使用它
add_subdirectory(lib)
add_subdirectory(app)

