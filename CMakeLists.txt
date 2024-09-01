cmake_minimum_required( VERSION 3.24 )

project( C78 LANGUAGES C )

if( WIN32 )
    set( C_COMPILE_FLAGS
                    /std:c90
                    /permissive-
                    /W4 
        )
endif()

add_executable( prog main.c )

message( STATUS "C compiler: " ${CMAKE_C_COMPILER_ID}"-"${CMAKE_C_COMPILER_VERSION} )