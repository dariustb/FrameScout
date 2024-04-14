set(CMAKE_INCLUDE_CURRENT_DIR ON)

add_executable(
        framescout
        framescout.m.cpp
)


add_library(framescout_core)
add_subdirectory(core)

target_link_libraries(framescout_core ${OpenCV_LIBS})
target_link_libraries(framescout PUBLIC
        framescout_core
)
