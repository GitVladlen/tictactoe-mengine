CMAKE_MINIMUM_REQUIRED(VERSION 3.0)

OPTION(MENGINE_DOWNLOADS_SILENT "Mengine download silent" OFF)

PROJECT(Downloads)

SET(MENGINE_REPOSITORY ${CMAKE_CURRENT_SOURCE_DIR}/../..)
SET(THIRDPARTY_DIR ${MENGINE_REPOSITORY}/dependencies)

include(download_template.cmake)

GIT_CLONE(Mengine https://github.com/irov/Mengine.git)

