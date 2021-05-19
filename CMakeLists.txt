cmake_minimum_required(VERSION 2.8.3)
project(eurobench_uneven_terrain)

SET(CMAKE_CXX_FLAGS "-std=c++0x ${CMAKE_CXX_FLAGS}")

foreach(dir launch models worlds urdf meshes)
    install(DIRECTORY ${dir}/
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)

