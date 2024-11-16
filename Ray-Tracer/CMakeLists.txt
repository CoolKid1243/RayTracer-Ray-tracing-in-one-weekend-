cmake_minimum_required(VERSION 3.1.0)
project(RayTracer VERSION 3.0.0 LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 11)

# Add the src directory to the include path
include_directories(${CMAKE_SOURCE_DIR}/src)
include_directories(${CMAKE_SOURCE_DIR}/src/HeaderFiles)
include_directories(${CMAKE_SOURCE_DIR}/src/HeaderFiles/Camera)

# Create executable
add_executable(RayTracer src/main.cc)
