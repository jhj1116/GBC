cmake_minimum_required(VERSION 3.5.1)
project(calculator)
include_directories(../ ../operand ../operator)
add_library(parser STATIC Parser.cpp Postfix.cpp)
target_link_libraries(parser calculator operand operator)
