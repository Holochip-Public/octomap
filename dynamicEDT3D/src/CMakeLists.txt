
add_library(dynamicedt3d SHARED dynamicEDT3D.cpp)
set_target_properties(dynamicedt3d PROPERTIES
  VERSION ${DYNAMICEDT3D_VERSION}
  SOVERSION ${DYNAMICEDT3D_SOVERSION}
)
target_link_libraries(dynamicedt3d PUBLIC ${OCTOMAP_LIBRARIES})
target_include_directories(dynamicedt3d PUBLIC ${CMAKE_CURRENT_LIST_DIR}/../include)
