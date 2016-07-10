cmake_minimum_required(VERSION 2.8.7)

project(cmake-test)

find_package(TinyCNN)

message(STATUS ${TINYCNN_FOUND})
message(STATUS ${TINYCNN_VERSION})
message(STATUS ${TINYCNN_INCLUDE_DIRS})
message(STATUS ${TINYCNN_LIBRARIES})
