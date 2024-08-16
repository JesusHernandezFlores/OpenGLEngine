cmake_minimum_required(VERSION 3.5.0)
project(OpenGLEngine VERSION 0.1.0 LANGUAGES C CXX)
include_directories(${CMAKE_SOURCE_DIR}/3rdParty/include)
link_directories(${CMAKE_SOURCE_DIR}/3rdParty/lib)

add_executable(OpenGLEngine src/main.cpp src/glad.c)
target_link_libraries(OpenGLEngine glfw3.a)

