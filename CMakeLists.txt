cmake_minimum_required(VERSION 3.0)
project(prover_benchmark)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)

add_executable(prover_benchmark src/main.cpp)

