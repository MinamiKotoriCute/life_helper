cmake_minimum_required(VERSION 3.5)

project(life_helper LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fcoroutines")

set(life_helper_src
    main.cpp
)

add_executable(life_helper
    ${life_helper_src}
)

target_link_libraries(life_helper
    PRIVATE
        hamtaro
)

target_include_directories(life_helper
    PRIVATE
        hamtaro
)
