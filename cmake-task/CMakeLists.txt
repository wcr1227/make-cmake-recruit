cmake_minimum_required(VERSION 3.10)
project(calculator)

add_executable(calculator
    src/main.c
    src/calculator.c
)

target_include_directories(calculator PRIVATE include)