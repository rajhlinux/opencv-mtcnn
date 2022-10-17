cmake_minimum_required(VERSION 3.2)

project (MTCNN C CXX)

set_property (GLOBAL PROPERTY USE_FOLDERS ON)

set (CMAKE_CXX_STANDARD 11)
set (CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Boost COMPONENTS filesystem REQUIRED)

include_directories(${Boost_INCLUDE_DIRS})


add_subdirectory (lib)
add_subdirectory (sample)

enable_testing()
