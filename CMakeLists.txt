cmake_minimum_required(VERSION 3.15)
project(MojDuzyProjekt)

set(CMAKE_CXX_STANDARD 20)

# Automatycznie zbiera wszystkie pliki .cpp z folderu src
file(GLOB_RECURSE SOURCES "src/*.cpp")

add_executable(${PROJECT_NAME} ${SOURCES})
target_include_directories(${PROJECT_NAME} PRIVATE include)