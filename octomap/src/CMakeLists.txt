add_subdirectory(math)

add_library( octomap SHARED
        AbstractOcTree.cpp
        AbstractOccupancyOcTree.cpp
        Pointcloud.cpp
        ScanGraph.cpp
        CountingOcTree.cpp
        OcTree.cpp
        OcTreeNode.cpp
        OcTreeStamped.cpp
        ColorOcTree.cpp
)
target_include_directories(octomap PUBLIC ${CMAKE_CURRENT_LIST_DIR}/../include)
target_link_libraries(octomap PUBLIC octomath)
