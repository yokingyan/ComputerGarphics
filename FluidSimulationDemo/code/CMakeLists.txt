cmake_minimum_required(VERSION 3.2 FATAL_ERROR)
project(FluidSimulationDemo VERSION 1.0)
message(STATUS "[Project] ${PROJECT_NAME} ${PROJECT_VERSION}")

include(cmake/helper.cmake)

set(OUTPUT_PROP   
    RUNTIME_OUTPUT_DIRECTORY_DEBUG          "${CMAKE_SOURCE_DIR}/bin"
    RUNTIME_OUTPUT_DIRECTORY_RELWITHDEBINFO "${CMAKE_SOURCE_DIR}/bin"
    RUNTIME_OUTPUT_DIRECTORY_RELEASE        "${CMAKE_SOURCE_DIR}/bin"
)

add_compile_options(-std=c++11)

add_subdirectory(Fluid2D)