#CMakeLists.txt to build project using cmake
#run $cmake path/to/CMakeLists.txt

cmake_minimum_required( VERSION 2.6 )

project( GPGPU )

set( CMAKE_BUILD_TYPE Debug)

# FrameBufferObject
add_subdirectory( "${CMAKE_SOURCE_DIR}/FBO" 
  "${CMAKE_BINARY_DIR}/FBO-${CMAKE_BUILD_TYPE}" )
# ImageSimple
add_subdirectory( "${CMAKE_SOURCE_DIR}/ImageSimple" 
  "${CMAKE_BINARY_DIR}/ImageSimple-${CMAKE_BUILD_TYPE}" )
# TransformFeedback
add_subdirectory( "${CMAKE_SOURCE_DIR}/TransformFeedback" 
  "${CMAKE_BINARY_DIR}/TransformFeedback-${CMAKE_BUILD_TYPE}" )
