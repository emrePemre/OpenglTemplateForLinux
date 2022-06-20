cmake_minimum_required(VERSION 3.16.3)

project(Game)

include_directories("../include")
set( SOURCE
    "../src/main.cpp"

)

set( LIB
    "../lib/glad.c"
)

set( INCLUDE 
    "../include"
)
include_directories(${INCLUDE})

add_executable(${PROJECT_NAME} ${LIB} ${SOURCE})

target_link_libraries(${PROJECT_NAME} GL dl glfw)
