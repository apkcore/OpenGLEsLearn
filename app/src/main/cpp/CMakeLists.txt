cmake_minimum_required(VERSION 3.4.1)
add_library( # Sets the name of the library.
             native-lib

             SHARED

             native-lib.cpp )

find_library( # Sets the name of the path variable.
              log-lib
              log )

target_link_libraries(
                       native-lib
                       ${log-lib} )