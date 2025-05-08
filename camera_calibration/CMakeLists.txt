cmake_minimum_required(VERSION 3.5)
project(camera_calibration)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_python REQUIRED)

file(GLOB PYTHON_FILES src/*.py)

install(PROGRAMS ${PYTHON_FILES} 
  DESTINATION lib/${PROJECT_NAME} 
)

ament_package()

