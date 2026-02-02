cmake_minimum_required(VERSION 3.20)
project(SumaArreglosParalela LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenMP REQUIRED)

add_executable(suma_arreglos main.cpp)
target_link_libraries(suma_arreglos PRIVATE OpenMP::OpenMP_CXX)

