# CMake Hello World Project

This project demonstrates a basic setup for using CMake, a powerful build system generator that helps manage the build process across different platforms.

## Introduction to CMake

CMake is a tool that generates build files for various environments, such as Makefiles on macOS/Linux or Visual Studio project files on Windows, allowing code to be compiled consistently across platforms. It’s commonly used in C/C++ projects to simplify configuration and building.

## Key Components of CMake

1. **CMakeLists.txt**: This is the primary configuration file in a CMake project. Here, you define the project's details, source files, and build targets.
2. **Variables**: CMake allows setting variables to define project settings (e.g., `PROJECT_NAME`, `CMAKE_MINIMUM_REQUIRED_VERSION`) and to pass options in commands.
3. **Commands**: Key commands in CMake include:
   - `project()`: Defines the project name and metadata.
   - `add_executable()`: Specifies the output executable for the project.
   - `cmake_minimum_required()`: Sets the minimum compatible CMake version.

## How CMake Works

CMake reads the `CMakeLists.txt` file and generates platform-specific build files based on the environment:

- **Makefiles** on Unix-based systems, used with the `make` command to compile code.
- **Project files** for IDEs like Visual Studio or Xcode.

## Project Structure

This project consists of two files:

1. **hello.c**: Contains the "Hello, World!" source code.
2. **CMakeLists.txt**: Holds the CMake configuration for the project.

### hello.c
```c
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
