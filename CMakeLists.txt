cmake_minimum_required(VERSION 3.10)

project(bb)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

include_directories(include)
include_directories(/opt/homebrew/include)

find_library(MIKMOD
  NAMES mikmod
)
link_directories(/opt/homebrew/lib)
link_libraries(aa ${MIKMOD})

aux_source_directory(src SRC)
add_definitions(-DSOUNDDIR="${PROJECT_SOURCE_DIR}")
add_executable(bb ${SRC})
