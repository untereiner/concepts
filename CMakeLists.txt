cmake_minimum_required(VERSION 3.7.2 FATAL_ERROR)

project(concepts
	LANGUAGES CXX
	)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(main main.cpp)

target_compile_options(main PRIVATE -fconcepts)
