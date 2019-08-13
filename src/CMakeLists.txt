target_jnum_directory(libtestjnum ${CMAKE_CURRENT_LIST_DIR}/jnum)

target_include_directories(libtestjnum INTERFACE ${CMAKE_CURRENT_LIST_DIR}/include)
add_subdirectory(bin)
