cmake_minimum_required(VERSION 3.12)
project(OpenGLApp)

find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)
find_package(glm REQUIRED)
find_package(glfw3 REQUIRED)

add_executable(OpenGLApp main.cpp)

target_link_libraries(OpenGLApp
    PRIVATE
    OpenGL::GL
    GLEW::GLEW
    glm
    glfw
)

