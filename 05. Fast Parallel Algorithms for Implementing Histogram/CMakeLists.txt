# collect source files

file( GLOB  hdr *.hpp *.h )

SET (HW5_files main.cu student.cu reference_calc.cpp)

CUDA_ADD_EXECUTABLE(HW5 ${HW5_files} ${hdr})
