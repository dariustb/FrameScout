target_include_directories(framescout_core PUBLIC ./)

target_sources(framescout_core
 	PRIVATE
		framescout_imagesearch.cpp
)

target_link_libraries(framescout_core ${OpenCV_LIBS})
