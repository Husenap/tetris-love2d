cmake_minimum_required(VERSION 3.22)
project(tetris LANGUAGES C)

add_library(tetris SHARED libtetris/src/libtetris.c)
set_target_properties(tetris PROPERTIES
  LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib
  LIBRARY_OUTPUT_DIRECTORY_DEBUG ${PROJECT_SOURCE_DIR}/lib
  LIBRARY_OUTPUT_DIRECTORY_RELEASE ${PROJECT_SOURCE_DIR}/lib
  RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/lib
  RUNTIME_OUTPUT_DIRECTORY_DEBUG ${PROJECT_SOURCE_DIR}/lib
  RUNTIME_OUTPUT_DIRECTORY_RELEASE ${PROJECT_SOURCE_DIR}/lib)