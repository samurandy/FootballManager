cmake_minimum_required(VERSION 3.10)
project(FootballManager)
set(CMAKE_TOOLCHAIN_FILE "D:/C++/vcpkg/scripts/buildsystems/vcpkg.cmake" CACHE STRING "vcpkg toolchain file")

set(CMAKE_CXX_STANDARD 17)
add_executable(server src/main.cpp)

include_directories(D:/C++/vcpkg/installed/x64-windows/include)

