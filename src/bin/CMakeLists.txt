add_executable(test_jnum test_jnum.cpp)
target_link_libraries(test_jnum PUBLIC libtestjnum)
add_test(NAME test_jnum COMMAND test_jnum)
