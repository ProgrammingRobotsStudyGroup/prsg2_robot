cmake_minimum_required(VERSION 2.8.3)
project(prsg2_robot)

find_package(catkin REQUIRED COMPONENTS urdf xacro)

catkin_package(
   CATKIN_DEPENDS urdf xacro
)

install(DIRECTORY urdf
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(DIRECTORY launch
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(DIRECTORY param
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
