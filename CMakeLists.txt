cmake_minimum_required(VERSION 3.0)
project(bar VERSION 1.0.0 DESCRIPTION "the awesome bar application")
add_executable(bar bar.cpp)
target_link_libraries(bar foo)

include(GNUInstallDirs)
install(TARGETS bar RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR})
