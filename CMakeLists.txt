cmake_minimum_required( VERSION 3.10 )
project( PrimeTest
  VERSION 1.0 )

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_set_find_paths()

find_package( Prime REQUIRED CONFIG )

add_executable( PrimeTest src/PrimeTest.cpp )
target_link_libraries( PrimeTest Prime::Prime )
