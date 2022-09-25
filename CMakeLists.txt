#file(GLOB_RECURSE DIR_LIB_SRCS "*.c" "*.h")
#
#add_library(MCUPrintfLib ${DIR_LIB_SRCS})
project(MCUPrintfLib
        LANGUAGES C)

add_library(${PROJECT_NAME})
target_sources(${PROJECT_NAME}
        PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}/printf.c)
target_include_directories(${PROJECT_NAME} INTERFACE ${CMAKE_CURRENT_LIST_DIR})