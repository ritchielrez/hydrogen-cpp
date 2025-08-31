cmake_minimum_required(VERSION 3.20)

project(hydrogen)

set(CMAKE_CXX_STANDARD 20)

add_compile_options(-fsanitize=address)

add_executable(hydro src/main.cpp)
