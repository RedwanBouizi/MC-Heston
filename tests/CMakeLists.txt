cmake_minimum_required(VERSION 3.8)
project(MC)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE
        interface
        plot
        print
        )

set(LIBRARIES
        mc
        )

add_definitions("-Wall -O2")

add_executable(example ${SOURCE})
target_link_libraries(example ${LIBRARIES})
