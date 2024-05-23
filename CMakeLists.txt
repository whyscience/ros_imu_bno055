cmake_minimum_required(VERSION 2.8.3)
project(ros_imu_bno055)

find_package(catkin REQUIRED COMPONENTS
        rospy
        sensor_msgs
        std_srvs
)

catkin_package(
        #  INCLUDE_DIRS include
        #  LIBRARIES ros_imu_bno055
        CATKIN_DEPENDS rospy sensor_msgs
        #  DEPENDS system_lib
)

###########
## Build ##
###########

## Specify additional locations of header files
## Your package locations should be listed before other locations
include_directories(
        # include
        ${catkin_INCLUDE_DIRS}
)