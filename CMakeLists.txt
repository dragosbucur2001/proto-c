cmake_minimum_required(VERSION 3.24)
project(proto_c C)

set(CMAKE_C_STANDARD 11)

include_directories(includes)

add_executable(proto_c
        includes/proto.c
        src/main.c)
