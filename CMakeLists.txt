cmake_minimum_required(VERSION 2.8)
project( DisplayImage )
find_package( OpenCV REQUIRED )
add_executable( object object_detection.cpp )

add_executable( object_click object_detection_click.cpp )

target_link_libraries( object ${OpenCV_LIBS} )
target_link_libraries( object_click ${OpenCV_LIBS} )
