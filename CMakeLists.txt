


cmake_minimum_required(VERSION 3.10)

project( camera_calibration)

find_package(OpenCV REQUIRED)
find_package(VISP REQUIRED)
include_directories(${VISP_INCLUDE_DIRS})

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable( camera_calibration camera_calibration.cpp )

include_directories(${VISP_INCLUDE_DIRS})

target_link_libraries( camera_calibration ${OpenCV_LIBS} ${VISP_LIBRARIES})


 
