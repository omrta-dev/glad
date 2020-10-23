cmake_minimum_required(VERSION 3.0)
project(glad)

add_library(${PROJECT_NAME} include/glad/glad.h src/glad.c)

set_target_properties(${PROJECT_NAME} PROPERTIES ENABLE_EXPORTS 1)
set_target_properties(${PROJECT_NAME} PROPERTIES WINDOWS_EXPORT_ALL_SYMBOLS 1)

target_include_directories(${PROJECT_NAME} PUBLIC include/)