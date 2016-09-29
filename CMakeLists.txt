cmake_minimum_required(VERSION 3.3)

project(boost_functional)

add_library(boost_functional INTERFACE)

target_include_directories(boost_functional BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_functional DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
