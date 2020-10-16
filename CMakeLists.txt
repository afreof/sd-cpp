#-------------------------------
# PROJECT INFORMATION
#-------------------------------

cmake_minimum_required(VERSION 3.13)

project(sd-cpp VERSION 0.0.1 LANGUAGES C CXX)

option(BUILD_TESTS "Build and install tests (default OFF)" ON)
option(BUILD_CODE_GEN "Build and install interface stub code generator (default OFF)" ON)
set(TESTS_INSTALL_PATH "${CMAKE_CURRENT_BINARY_DIR}/rootfs")

add_subdirectory("${CMAKE_CURRENT_SOURCE_DIR}/sdbus-cpp")

