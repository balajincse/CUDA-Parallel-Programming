# collect source files

file( GLOB  hdr *.hpp *.h )
file( GLOB  cu  *.cu)
SET (HW4_files main.cpp loadSaveImage.cpp reference_calc.cpp compare.cpp)

CUDA_ADD_EXECUTABLE(HW4 ${HW4_files} ${hdr} ${img} ${cu})
