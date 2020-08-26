# CMakelists.txt
# 

# cmake 最低版本需求
cmake_minimum_required(VERSION 2.8)

# 项目名称(为项目启用C/C++/Fortran)
project(fdemo C CXX Fortran)

# aux_source_directory(. DIR_SRCS)

set(ALLBLAS allblas/lsame.f allblas/xerbla.f allblas/xerbla_array.f)

add_library(${PROJECT_NAME} ${ALLBLAS})









# add_library(${PROJECT_NAME} SHARED 1.f)
# add_library(${PROJECT_NAME} STATIC 1.f)

