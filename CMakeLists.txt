cmake_minimum_required(VERSION 2.8.7)

project(cmake-test)

find_package(TinyCNN)

message(STATUS ${TINYCNN_FOUND})
message(STATUS ${TINYCNN_VERSION})
message(STATUS ${TINYCNN_INCLUDE_DIRS})
message(STATUS ${TINYCNN_LIBRARIES})

include_directories(${TINYCNN_INCLUDE_DIRS})
add_executable(tiny_cnn_test main.cpp ${TINYCNN_INCLUDE_DIRS})
target_link_libraries(tiny_cnn_test ${TINYCNN_LIBRARIES})
