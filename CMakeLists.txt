cmake_minimum_required(VERSION 3.12)
cmake_policy(SET CMP0079 NEW)
list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake")
project(test_jnum)

find_package(jnum REQUIRED)

add_library(libtestjnum INTERFACE)
target_link_libraries(libtestjnum INTERFACE jnum::jnum)
include(CTest)
add_subdirectory(src)
