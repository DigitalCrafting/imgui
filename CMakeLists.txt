cmake_minimum_required (VERSION 3.16)
project(imgui)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

file(GLOB SOURCES_LIST "*.cpp" "*.hpp" "*.h")

add_library(${PROJECT_NAME} STATIC ${SOURCES_LIST})

target_include_directories(${PROJECT_NAME} PUBLIC ./)