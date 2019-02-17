project(lib_AtmosphereModel_project)

include_directories ("${PROJECT_SOURCE_DIR}/src")
include_directories ("${PROJECT_SOURCE_DIR}/..")

add_library(AtmosphereModel SHARED AtmosphereModel.c 
AtmosphereModel.h
)

install(TARGETS AtmosphereModel DESTINATION lib)
install(FILES AtmosphereModel.h DESTINATION include)
