cmake_minimum_required(VERSION 3.28.1)
project(Inhaler VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_executable(Inhaler src/main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
