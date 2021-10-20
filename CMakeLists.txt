cmake_minimum_required(VERSION 3.20)
project(ocl_tutorial)
find_package(OpenCL REQUIRED)
set(CMAKE_CXX_STANDARD 14)
include_directories(${CUDA_PATH}/include)
link_directories(${CUDA_PATH}/lib/x64)
add_executable(ocl_tutorial main.cpp)
target_link_libraries(ocl_tutorial OpenCL::OpenCL)

