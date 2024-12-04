cmake_minimum_required(VERSION 3.5.0)
project(p2p-tracker VERSION 0.1.0 LANGUAGES C CXX)

find_package(CURL CONFIG REQUIRED)

add_executable(p2p-tracker main.cpp)

target_link_libraries(p2p-tracker CURL::libcurl)

