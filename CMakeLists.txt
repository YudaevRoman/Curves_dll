cmake_minimum_required(VERSION 3.5.0)
project(Curves_dll VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_library(Curves_dll 
    Curves_dll.cpp
)

set(EXECUTABLE_OUTPUT_PATH "../bin")
set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
