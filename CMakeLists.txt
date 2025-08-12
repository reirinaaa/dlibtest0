cmake_minimum_required(VERSION 4.1.0)

project(dlibtest0)

# include(FetchContent)
# FetchContent_Declare(dlib GIT_REPOSITORY https://github.com/davisking/dlib.git GIT_TAG v20.0)
# FetchContent_MakeAvailable(dlib)

add_subdirectory(../dlib dlib_build)

add_executable(learning assignment_learning_ex.cpp)

target_link_libraries(learning dlib::dlib)
