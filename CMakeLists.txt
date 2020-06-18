cmake_minimum_required(VERSION 3.2)
project(VideoStablizationGPU)


FIND_PACKAGE(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDES})
include_directories(include)


FILE(GLOB
        src_file
        src/*.cpp
        )

add_executable(${PROJECT_NAME}
        ${src_file}

        )


target_link_libraries(
        ${PROJECT_NAME}
        ${OpenCV_LIBRARIES}

)