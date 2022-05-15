file(GLOB_RECURSE DIR_LIB_SRCS "*.c" "*.h")

add_library(MCUPrintfLib ${DIR_LIB_SRCS})