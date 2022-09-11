cmake_minimum_required(VERSION 3.15)
project(cmake_test VERSION 0.1.0)

include(CTest)
enable_testing()

#add_subdirectory(lib)
#add_subdirectory(include)

add_executable(cmake_test src/main.cpp)

set(CPACK_PROJECT_NAME $(PROJECT_NAME))
set(CPACK_PROJECT_VERSION $(PROJECT_VERSION))
include(CPack)

