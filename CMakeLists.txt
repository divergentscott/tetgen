# Set  the minimum  required version  of cmake  for a  project.
cmake_minimum_required(VERSION 2.6)
project(tetgen)

include_directories(${tetgen_SOURCE_DIR})

# Add an executable to the project using the specified source files.
add_executable(tetgen tetgen.cxx predicates.cxx)

#Add a library to the project using the specified source files. 
# In Linux/Unix, it will creates the libtet.a
#add_library(tet tetgen.cxx predicates.cxx)

# add_executable(ack ack.cxx tetgen.h)
# add_executable(ack ack.cxx tetgen.h)
# target_link_libraries(ack tet)


#Set properties on a target. 
#We use this here to set -DTETLIBRARY for when compiling the
#library
#set_target_properties(tet PROPERTIES "COMPILE_DEFINITIONS" TETLIBRARY)a
#add_definitions(-DTETLIBRARY)