cmake_minimum_required(VERSION 2.6)
project (Lab2)

set (SRC_LIST main.cpp)
set(HEADERS calculator.h)
set(SOURCES calculator.cpp)

add_library(lib ${SOURCES} ${HEADERS})
add_executable(${PROJECT_NAME} ${SRC_LIST})

target_link_libraries(${PROJECT_NAME} lib)

