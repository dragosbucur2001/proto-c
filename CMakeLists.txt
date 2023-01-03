cmake_minimum_required(VERSION 3.18)
project(proto_c C)

set(CMAKE_C_STANDARD 11)

include_directories(includes)

add_compile_options(-Wall -Wextra -pedantic -Werror)

add_executable(server src/server.c)
add_executable(client src/client.c)

# target_compile_options(client PUBLIC "$<$<CONFIG:RELEASE>:-O2>")
# target_compile_options(server PUBLIC "$<$<CONFIG:RELEASE>:-O2>")
