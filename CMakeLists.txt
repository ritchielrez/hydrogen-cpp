cmake_minimum_required(VERSION 3.20)

project(hydrogen)

set(CMAKE_CXX_STANDARD 20)

add_executable(hydro src/main.cpp)

if(MSVC)
  target_compile_options(hydro PRIVATE /W4 /WX)
else()
  target_compile_options(hydro PRIVATE -Wall -Wextra -Wpedantic -Werror)
endif()