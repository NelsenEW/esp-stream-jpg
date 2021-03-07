# The following lines of boilerplate have to be in your project's CMakeLists
# in this exact order for cmake to work correctly
cmake_minimum_required(VERSION 3.5)

set(__PROJECT_GROUP_LINK_COMPONENTS ON)

include($ENV{IDF_PATH}/tools/cmake/project.cmake)
set(EXTRA_COMPONENT_DIRS "./esp32-camera")
project(esp32_cam_http_jpg_stream)
