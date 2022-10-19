cmake_minimum_required(VERSION 3.19.0)

add_library(oldmfc INTERFACE)
target_compile_definitions(oldmfc INTERFACE _AFX_NOFORCE_LIBS)
target_link_libraries(oldmfc INTERFACE mfc42)
target_link_directories(oldmfc BEFORE INTERFACE lib)
target_include_directories(oldmfc INTERFACE include)
