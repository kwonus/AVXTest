cmake_minimum_required (VERSION 3.19)
project (AVXTest)
#set(CMAKE_PREFIX_PATH "C:/CMake/public")

include_directories("C:/Users/kevin/source/C/XVMem;C:/Users/kevin/source/C/AVXLib")
link_directories("C:/Users/kevin/source/C/XVMem/out/build/x64-Debug;C:/Users/kevin/source/C/AVXLib/out/build/x64-Debug")
find_library(XVMEM_LIB XVMem)
find_library(AVX_LIB AVXLib)
link_libraries(XVMem AVXLib)

# Add source to this project's executable.
add_executable (AVXTest AVXTest.cpp)
