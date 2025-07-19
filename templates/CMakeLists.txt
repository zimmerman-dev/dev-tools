cmake_minimum_required(VERSION 3.16)

# Name of the project
project(my_project LANGUAGES CXX)

# Require modern C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# Add executable (manually list your main source file)
add_executable(${PROJECT_NAME}
    src/main.cpp
)

# Optional: Add include directory if you have headers
target_include_directories(${PROJECT_NAME}
    PRIVATE
        include
)
