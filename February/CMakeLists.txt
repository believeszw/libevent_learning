project(February)

SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/../bin/${COMPILE_PLAT})

aux_source_directory(. DIR_SRCS)

SET(TEST_LIB gtest gtest_main -lpthread)

add_executable(FebruaryTest ${DIR_SRCS})

target_link_libraries(FebruaryTest ${TEST_LIB})
INSTALL(TARGETS FebruaryTest DESTINATION ${EXECUTABLE_OUTPUT_PATH})