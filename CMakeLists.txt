# bisc/
cmake_minimum_required (VERSION 3.8)

project("bisc")

add_library(bisc STATIC "include/bisc.hpp" "src/dummy.cpp")

set_property(TARGET bisc PROPERTY LINKER_LANGUAGE CXX)

target_include_directories(bisc PUBLIC "include")
