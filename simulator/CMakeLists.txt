cmake_minimum_required(VERSION 3.21)
project(simulator)
set(CMAKE_CXX_STANDARD 14)


add_executable(simulator
	main.cpp
	)

target_include_directories(simulator PRIVATE
	${CMAKE_SOURCE_DIR}
	)
