cmake_minimum_required(VERSION 3.20)
project(hello-wave)
set(CMAKE_CXX_STANDARD 20)

add_executable(hello-wave "src/hello-wave.cpp")

add_subdirectory("dependencies/portaudio")
target_link_libraries(hello-wave PRIVATE PortAudio)
