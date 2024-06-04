cmake_minimum_required(VERSION 3.27)
project(dev_lib)

set(CMAKE_CXX_STANDARD 23)

add_library(dev_lib INTERFACE
        include/reflect.h
        include/proxy.h
)
#
#add_library(dev_lib_static STATIC
#        include/reflect.h
#        include/proxy.h)

add_executable(reflect_test src/reflect_test.cpp
)

add_executable(proxy_test src/proxy_test.cpp
)

#target_link_libraries(main dev_lib)

