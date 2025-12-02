cmake_minimum_required(VERSION 3.16)

project({{project_name}}
    VERSION 0.1.0
    DESCRIPTION "{{project_description}}"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD {{cpp_standard}})
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# Common scenario: fmt is discoverable via find_package(fmt)
# - system: install fmt (e.g. apt/yum/pacman/brew)
# - vcpkg: use vcpkg toolchain + fmt port
# - conan: use cmake_find_package / CMakeDeps generators

find_package(fmt REQUIRED)

add_executable({{project_name}}
    src/main.cpp
)

target_link_libraries({{project_name}}
    PRIVATE
        fmt::fmt
)

target_compile_features({{project_name}} PRIVATE cxx_std_{{cpp_standard}})

