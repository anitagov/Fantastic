# Top-level CMake file (sample)
cmake_minimum_required(VERSION 3.5.1)
project (Fantastic)

# The version number.
set (Fantastic_VERSION_MAJOR 1)
set (Fantastic_VERSION_MINOR 0)

# configure a header file to pass some of the CMake settings
# to the source code
configure_file (
  "${PROJECT_SOURCE_DIR}/FantasticConfig.h.in"
  "${PROJECT_BINARY_DIR}/FantasticConfig.h"
  )

# add the binary tree to the search path for include files
# so that we will find FantasticConfig.h
include_directories("${PROJECT_BINARY_DIR}")

add_executable (Fantastic Fantastic.cpp)
