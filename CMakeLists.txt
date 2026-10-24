
cmake_minimum_required(VERSION 3.16)

project(TaskManager LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(task_manager
    src/main.cpp
    src/task_manager.cpp
)

target_include_directories(task_manager
    PRIVATE ${PROJECT_SOURCE_DIR}/include
)