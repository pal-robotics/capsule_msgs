cmake_minimum_required(VERSION 2.8.3)
project(capsule_msgs)

find_package(catkin REQUIRED geometry_msgs message_generation)

add_message_files(
  FILES
    Capsule.msg
)

generate_messages(
  DEPENDENCIES
    geometry_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime geometry_msgs
)
