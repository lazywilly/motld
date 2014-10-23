cmake_minimum_required( VERSION 2.8.8 )

project( motld )

find_package( OpenCV REQUIRED )

include_directories( "${CMAKE_CURRENT_SOURCE_DIR}" )

add_executable( camExample camExample.cpp )

target_link_libraries( camExample ${OpenCV_LIBS} )