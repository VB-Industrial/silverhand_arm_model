cmake_minimum_required(VERSION 3.16)
project(silverhand_arm_model)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY launch meshes rviz urdf
  DESTINATION share/${PROJECT_NAME}
  PATTERN "__pycache__" EXCLUDE
  PATTERN "*.pyc" EXCLUDE
  PATTERN "*.urdf" EXCLUDE
)

ament_package()
