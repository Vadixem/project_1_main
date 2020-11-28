cmake_minimum_required( VERSION 3.0 )

project( project_1_main )

#find_package( project_1_lib REQUIRED )
add_subdirectory( ${CMAKE_CURRENT_SOURCE_DIR}/submodules/project_1_lib )

add_executable( project_1_main main.cpp )

target_link_libraries( project_1_main PUBLIC project_1_lib )
