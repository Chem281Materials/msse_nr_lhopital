cmake_minimum_required(VERSION 3.14)

# Project name and version
project(Limit VERSION 1.0
	          DESCRIPTION "Evaluation of a numerical limit"
		      LANGUAGES CXX)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

# Add the executable
add_executable(limit src/main.cpp)
