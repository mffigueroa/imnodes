cmake_minimum_required(VERSION 3.20)

project(ImNodes)

find_package(imgui CONFIG REQUIRED)

add_library(imnodes STATIC imnodes.cpp)
target_link_libraries(imnodes PRIVATE imgui::imgui)
target_include_directories(imnodes PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})