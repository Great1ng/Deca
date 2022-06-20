cmake_minimum_required(VERSION 3.22)

project(Deca)

include(cmake/CompileOptions.cmake)
include(cmake/Development.cmake)
include(cmake/Sanitize.cmake)
include(cmake/SFMLOptions.cmake)

add_subdirectory(SFML)
add_executable(Deca deca.cpp)
target_link_libraries(Deca sfml-graphics sfml-window)