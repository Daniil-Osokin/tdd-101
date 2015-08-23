set(target ${PROJECT_LIBRARY})

FILE(GLOB hdrs "*.h*" "${PROJECT_INCLUDE}/*.h*")
FILE(GLOB srcs "*.cpp")

ADD_LIBRARY(${target} STATIC ${srcs} ${hdrs})
