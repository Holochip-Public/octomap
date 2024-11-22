add_library( octomath STATIC
        Vector3.cpp
        Quaternion.cpp
        Pose6D.cpp
)
target_include_directories(octomath PUBLIC ${CMAKE_CURRENT_LIST_DIR}/../../include)

SET_TARGET_PROPERTIES( octomath PROPERTIES
  VERSION ${OCTOMAP_VERSION}
  SOVERSION ${OCTOMAP_SOVERSION}
)
