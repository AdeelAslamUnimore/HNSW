cmake_minimum_required(VERSION 3.10)

# Project name
project(HNSW)

# Set C++ standard
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Include directories
include_directories(${PROJECT_SOURCE_DIR})

# Source files
set(SOURCES
    hnsw.cpp
    main.cpp
)

# Create executable
add_executable(hnsw_main ${SOURCES})

# Link libraries (if any, e.g., math library)
target_link_libraries(hnsw_main m)
