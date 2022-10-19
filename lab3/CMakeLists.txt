cmake_minimum_required(VERSION 2.8)	
 				
project(lab3)			

set(SOURCE_EXE main.cpp)		

set(SOURCE_LIB factorial.cpp hello.cpp)			

add_library(functions STATIC ${SOURCE_LIB})	

add_executable(main ${SOURCE_EXE})	

target_link_libraries(main functions)	
