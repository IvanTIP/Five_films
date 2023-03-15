cmake_minimum_required(VERSION 3.20)
project(ex2)

set(CMAKE_CXX_STANDARD 14)

set(JSON_BuildTests OFF CACHE INTERNAL "")

add_subdirectory(nlohmann_json)

add_executable(ex2 main.cpp)

target_link_libraries(ex2 PRIVATE nlohmann_json::nlohmann_json)