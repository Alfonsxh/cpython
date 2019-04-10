add_executable(python3.8 python.c ../Modules/main.c)

target_link_libraries(python3.8
        alfons_object
        alfons_python
        alfons_module
        alfons_parser
        crypt
        pthread
        dl
        util
        m)