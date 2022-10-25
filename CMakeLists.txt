cmake_minimum_required(VERSION 3.2.2)
project(CvEllipseFitExp)
set(CMAKE_C_COMPILER gcc.exe)
set(CMAKE_CXX_COMPILER g++.exe)

# Set opencv directory where you build opencv using mingw
set(OpenCV_DIR D:/opencv340/GccBuildContrib)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(CvEllipseFitExp CvEllipseFitExp.cpp)
target_link_libraries(CvEllipseFitExp  ${OpenCV_LIBS})