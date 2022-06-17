cmake_minimum_required(VERSION 3.0)
project(eigen3-minimal)
 
find_package(Eigen3 3.3 REQUIRED NO_MODULE)
 
add_executable(${CMAKE_PROJECT_NAME} src/main.cpp)
target_link_libraries(${CMAKE_PROJECT_NAME} Eigen3::Eigen)
