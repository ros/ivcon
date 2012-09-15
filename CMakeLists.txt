cmake_minimum_required(VERSION 2.8)
project(ivcon)

find_package(catkin REQUIRED)

catkin_stack()
catkin_project(${PROJECT_NAME})

add_executable(${PROJECT_NAME} src/ivcon.cpp)
target_link_libraries(${PROJECT_NAME} m)

install(TARGETS ${PROJECT_NAME}
  RUNTIME DESTINATION bin)
