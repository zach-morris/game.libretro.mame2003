cmake_minimum_required(VERSION 3.1)
project(game.libretro.mame2003)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR})

find_package(Kodi REQUIRED)
find_package(libretro-mame2003 REQUIRED)

set(MAME2003_CUSTOM_BINARY ${MAME2003_LIB}
    ${PROJECT_NAME}${CMAKE_SHARED_LIBRARY_SUFFIX})

build_addon(${PROJECT_NAME} MAME2003 "")
