# this one should build the executable menge and include the library builds
# TODO: should it build the plugins as well?

cmake_minimum_required(VERSION 3.12)

add_subdirectory(src/Menge/MengeCore)
add_subdirectory(src/Menge/MengeVis)
add_subdirectory(src/Plugins) #this could actually be a separate project that actually depends on mengeCore and/or mengeVis, i.e.

add_executable(menge src/Menge/mengeMain/mengeMain.cpp)
