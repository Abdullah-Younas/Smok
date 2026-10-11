# Smok

**Smok** is an experimental programming language and interpreter built from scratch in C++.

The goal of this project is to explore the internals of programming languages by building the core components of an interpreter, including lexical analysis, parsing, abstract syntax trees, variable environments, and execution.

## Overview

Smok is being developed as a learning project to understand how source code is transformed into executable behavior.

The interpreter is organized into independent components, each responsible for a different stage of the interpretation process.

## Project Structure

```text
smok/
├── CMakeLists.txt
├── README.md
├── src/
│   ├── main.cpp
│   ├── Lexer.cpp
│   ├── Token.cpp
│   ├── Parser.cpp
│   ├── AST.cpp
│   ├── Interpreter.cpp
│   └── Environment.cpp
├── include/
│   ├── Token.h
│   ├── Lexer.h
│   ├── Parser.h
│   ├── AST.h
│   ├── Interpreter.h
│   └── Environment.h
├── tests/
└── examples/
    ├── hello.ml
    └── arithmetic.ml
```

## Architecture

- **Lexer:** Converts source text into tokens.
- **Token:** Represents individual language elements, such as identifiers, literals, and operators.
- **Parser:** Analyzes tokens and constructs a representation of the program's syntax.
- **AST:** Defines the abstract syntax tree used to represent program structure.
- **Environment:** Manages variable bindings and execution scopes.
- **Interpreter:** Evaluates program representations and executes instructions.

## Tech Stack

- C++
- C++17
- CMake
- Linux

## Getting Started

### Prerequisites

Install a C++ compiler, CMake, and Git.

On Debian-based Linux distributions, including Ubuntu and Linux Mint:

```bash
sudo apt update
sudo apt install build-essential cmake git
```

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/smok.git
cd smok
```

Replace `YOUR_USERNAME` with your GitHub username.

### Build

```bash
cmake -S . -B build
cmake --build build
```

### Run

```bash
./build/smok
```

## Examples

Example Smok programs are stored in the `examples/` directory.

- `hello.sk`
- `arithmetic.sk`

Language syntax and supported features will evolve as development progresses.

## Development Status

Smok is a work in progress. Its lexer, parser, AST, environment, and interpreter components are being developed incrementally.

Features and syntax will be documented as they are implemented.

## Goals

- Build an interpreter from the ground up in C++.
- Understand lexical analysis, parsing, and AST construction.
- Explore variable storage, environments, and scope.
- Implement expression evaluation and program execution.
- Develop a simple and understandable language architecture.

## License

No license has been specified yet. Until one is added, all rights are reserved by default. If you intend to make Smok open source, consider adding an appropriate license.

---

Built from scratch with C++ and curiosity.
