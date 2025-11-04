cmake_minimum_required(VERSION 3.15)
project(IndustrialMonitor)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_TOOLCHAIN_FILE "${CMAKE_CURRENT_SOURCE_DIR}/vcpkg/scripts/buildsystems/vcpkg.cmake"
  CACHE STRING "Vcpkg toolchain file")

find_package(Crow CONFIG REQUIRED)
find_package(nlohmann_json CONFIG REQUIRED)

add_executable(server src/main.cpp)

target_link_libraries(server PRIVATE crow::crow nlohmann_json::nlohmann_json)