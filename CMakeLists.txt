cmake_minimum_required(VERSION 3.13)

add_compile_definitions(Py_BUILD_CORE)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/Include ${CMAKE_CURRENT_SOURCE_DIR}/Include/internal ${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(Python)
add_subdirectory(Objects)
add_subdirectory(Modules)
add_subdirectory(Parser)
add_subdirectory(Programs)
