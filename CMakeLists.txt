cmake_minimum_required(VERSION 3.16)
project(Million_Mobarmeg_Masry)

add_executable(Million_Mobarmeg_Masry main.cpp)

install(
    TARGETS Million_Mobarmeg_Masry
    RUNTIME
    DESTINATION bin
)

#
# CPACK macros below here
#
set(CPACK_PACKAGE_NAME "Million_Mobarmeg_Masry")
set(CPACK_PACKAGE_VENDOR "Iyad Ahmed")
set(CPACK_PACKAGE_DESCRIPTION_SUMMARY "CMake Installer Example")
set(CPACK_PACKAGE_VERSION "1.0.1")
set(CPACK_PACKAGE_VERSION_MAJOR "1")
set(CPACK_PACKAGE_VERSION_MINOR "0")
set(CPACK_PACKAGE_VERSION_PATCH "1")
set(CPACK_PACKAGE_INSTALL_DIRECTORY "CPack Installer Example")

set(CPACK_PACKAGE_EXECUTABLES Million_Mobarmeg_Masry "Million_Mobarmeg_Masry")
set(CPACK_CREATE_DESKTOP_LINKS Million_Mobarmeg_Masry)
set(CPACK_NSIS_MODIFY_PATH "ON")

# Must be after the last CPACK macros
include(CPack)
