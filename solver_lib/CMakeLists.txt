cmake_minimum_required(VERSION 3.4)

project(Solver)

set(CMAKE_CXX_STANDARD 11)

set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_library(solver STATIC /home/olga/olgaGor03/workspace/projects/lab03/lab03/solver_lib/solver.cpp /home/olga/olgaGor03/workspace/projects/lab03/lab03/formatter_ex_lib/formatter_ex.cpp /home/olga/olgaGor03/workspace/projects/lab03/lab03/formatter_lib/formatter.cpp)
include_directories(/home/olga/olgaGor03/workspace/projects/lab03/lab03/solver_lib /home/olga/olgaGor03/workspace/projects/lab03/lab03/formatter_ex_lib /home/olga/olgaGor03/workspace/projects/lab03/lab03/formatter_lib)
add_executable(Solver /home/olga/olgaGor03/workspace/projects/lab03/lab03/solver_application/equation.cpp)
target_link_libraries(Solver solver)
