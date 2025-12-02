cmake_minimum_required(VERSION 3.16)

project({{project_name}}
    VERSION 0.1.0
    DESCRIPTION "{{project_description}} (no external dependencies)"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD {{cpp_standard}})
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable({{project_name}}
    src/main.cpp
)

target_compile_features({{project_name}} PRIVATE cxx_std_{{cpp_standard}})
