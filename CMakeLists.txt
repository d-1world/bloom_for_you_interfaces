cmake_minimum_required(VERSION 3.8)
project(bloom_for_you_interfaces)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "msg/Command.msg"
  "msg/FlowerInfo.msg"
)

ament_package()
