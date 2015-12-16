PROJECT(MyHello)
cmake_minimum_required(VERSION 2.8)

include(conanbuildinfo.cmake)
CONAN_BASIC_SETUP()

ADD_EXECUTABLE(test test.c)
include_directories(${CONAN_INCLUDE_DIRS})
target_link_libraries(test ${CONAN_LIBS})

