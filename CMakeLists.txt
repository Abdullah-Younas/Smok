cmake_minimum_required(VERSION 3.16)

project(Smok LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(smok
    src/main.cpp
    src/Token.cpp
    src/Lexer.cpp
    src/Parser.cpp
    src/AST.cpp
    src/Interpreter.cpp
    src/Environment.cpp
)

target_include_directories(smok PRIVATE include)

target_compile_options(smok PRIVATE
    -Wall
    -Wextra
    -Wpedantic
)
