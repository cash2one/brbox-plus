cmake_minimum_required(VERSION 2.8.9)
set(PROJECT_NAME BrBoxComponents)
project(${PROJECT_NAME})
add_subdirectory(lib)
add_subdirectory(services)

#for cross compiling
#cmake -H. -BOutput -DCMAKE_TOOLCHAIN_FILE=/path/to/toolchain-arm-backup.cmake -DCMAKE_INSTALL_PREFIX=/home/user/tmp/
#cmake --build Output -- all
#cmake --build Output -- install

#for local compiling
#cmake -H. -BOutput
#cmake --build Output -- all

#for cleaning make generated output
#rm -rf Output

