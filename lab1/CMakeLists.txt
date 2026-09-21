cmake_minimum_required(VERSION 3.10.0)
project(lab1 VERSION 0.1.0 LANGUAGES C CXX)

set(OpenCV_DIR "D:/School/formafelismeres/opencv/opencv/build")   # adjust this path to your OpenCV install
find_package(OpenCV REQUIRED)
add_executable(lab1 main.cpp)



target_include_directories(lab1 PRIVATE ${OpenCV_INCLUDE_DIRS})
target_link_libraries(lab1 PRIVATE ${OpenCV_LIBS})