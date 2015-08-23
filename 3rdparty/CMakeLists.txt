SET(gtest_target "gtest")

FIND_PACKAGE(Threads)

FILE(GLOB srcs "gtest/*.cc")

ADD_LIBRARY(${gtest_target} STATIC ${srcs})

TARGET_LINK_LIBRARIES(${gtest_target} ${CMAKE_THREAD_LIBS_INIT})
