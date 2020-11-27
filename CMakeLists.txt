cmake_minimum_required( VERSION 3.0 )

find_package( project_1_lib )

add_executable( project_1_main main.cpp )

target_link_libraries( project_1_main project_1_lib::project_1_lib )