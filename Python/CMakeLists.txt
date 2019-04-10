include_directories(${CMAKE_CURRENT_SOURCE_DIR}/clinic)

add_compile_definitions(SOABI="cpython-38m-x86_64-linux-gnu")

aux_source_directory(. PYTHON_SRCS)
list(REMOVE_ITEM PYTHON_SRCS ./dynload_aix.c ./dynload_dl.c ./dynload_hpux.c ./dynload_stub.c ./dynload_win.c)

add_library(alfons_python ${PYTHON_SRCS})