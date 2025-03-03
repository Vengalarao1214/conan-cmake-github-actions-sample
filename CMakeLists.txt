cmake_minimum_required(VERSION 3.15)
project(SampleProject)

add_executable(sample_app src/main.cpp)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

target_link_libraries(sample_app ${CONAN_LIBS})
