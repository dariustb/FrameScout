set(CMAKE_INCLUDE_CURRENT_DIR ON)

add_executable(
        framescout
        framescout.m.cpp
)

target_link_libraries(framescout ${OpenCV_LIBS})

add_library(framescout_core)
add_subdirectory(core)

