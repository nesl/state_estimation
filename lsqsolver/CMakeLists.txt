cmake_minimum_required(VERSION 2.8)

project(path-refinement)

find_package(Ceres REQUIRED)
include_directories(${CERES_INCLUDE_DIRS})

# helloworld
add_executable(refine refine_path.cpp)
target_link_libraries(refine ${CERES_LIBRARIES})