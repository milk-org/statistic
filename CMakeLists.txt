project(lib_statistic_project)

include_directories ("${PROJECT_SOURCE_DIR}/src")
include_directories ("${PROJECT_SOURCE_DIR}/..")
add_library(statistic SHARED statistic.c)

install(TARGETS statistic DESTINATION lib)
install(FILES statistic.h DESTINATION include)

