cmake_minimum_required(VERSION 2.8.3)
project(rosnode)
find_package(catkin REQUIRED)
catkin_package()

catkin_python_setup()

if(CATKIN_ENABLE_TESTING)
  find_package(rostest)
  add_rostest(test/rosnode.test)
endif()
