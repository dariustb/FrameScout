add_executable(test_framescout)
target_link_libraries(test_framescout
	PUBLIC
		GTest::gtest_main
		framescout_core
)

target_sources(test_framescout
	PRIVATE
		framescout_frame.t.cpp
)

include(GoogleTest)
gtest_discover_tests(test_framescout)

