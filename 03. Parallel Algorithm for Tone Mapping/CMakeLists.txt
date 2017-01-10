# minimum required cmake version
cmake_minimum_required(VERSION 2.8)
find_package(CUDA QUIET REQUIRED)

SET (compare_files compare.cpp)

file( GLOB  hdr *.hpp *.h )
file( GLOB  cu  *.cu)
SET (HW3_files main.cpp loadSaveImage.cpp reference_calc.cpp compare.cpp)

CUDA_ADD_EXECUTABLE(HW3 ${HW3_files} ${hdr} ${cu})
