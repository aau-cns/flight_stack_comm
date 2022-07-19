cmake_minimum_required(VERSION 3.0.2)
project(flightstack_comm)

find_package(catkin REQUIRED COMPONENTS actionlib_msgs message_generation std_msgs)

add_message_files(
  DIRECTORY msg
  FILES
)

add_service_files(
  DIRECTORY srv
  FILES
)

add_action_files(
  DIRECTORY action
  FILES
)

generate_messages(
  DEPENDENCIES actionlib_msgs std_msgs
)

catkin_package(
  CATKIN_DEPENDS actionlib_msgs message_runtime
)
