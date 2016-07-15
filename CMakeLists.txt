cmake_minimum_required(VERSION 2.8.7)

project(cmake-test)

set(TinyCNN_USE_TBB ON)
find_package(TinyCNN)

message(STATUS ${TINYCNN_FOUND})
message(STATUS ${TinyCNN_VERSION})
message(STATUS ${TinyCNN_INCLUDE_DIRS})
message(STATUS ${TinyCNN_LIBRARIES})

set(CMAKE_CXX_STANDARD 11)

add_executable(tiny_cnn_test main.cpp)
target_link_libraries(tiny_cnn_test ${TinyCNN_LIBRARIES})
