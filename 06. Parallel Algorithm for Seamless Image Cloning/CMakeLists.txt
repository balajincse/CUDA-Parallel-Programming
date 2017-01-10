# collect source files

file( GLOB  hdr *.hpp *.h )

SET (HW6_files student_func.cu HW6.cu main.cpp loadSaveImage.cpp reference_calc.cpp compare.cpp)

CUDA_ADD_EXECUTABLE(HW6 ${HW6_files} ${hdr})
