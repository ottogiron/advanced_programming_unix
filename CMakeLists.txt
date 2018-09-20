cmake_minimum_required (VERSION 3.12.2)
project (AdvancedProgrammingUnix)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# add the binary tree to the search path for include files
# so that we will find TutorialConfig.h
include_directories("${PROJECT_BINARY_DIR}")
include_directories("apue.3e/include")

#link directories
link_directories("apue.3e/lib")

add_executable(adv ch03/test_seek.c)
