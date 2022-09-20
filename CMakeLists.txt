option(BUILD_THORMANG3_SAMPLES "Building THORMANG3 sampels" ON)
if(NOT BUILD_THORMANG3_SAMPLES)
  return()
endif()

install(DIRECTORY model DESTINATION ${CHOREONOID_SHARE_SUBDIR}/THORMANG3)

add_subdirectory(ThormanG3Controller)
