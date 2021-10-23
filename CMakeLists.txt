cmake_minimum_required(VERSION 3.5)
project(cutefish-icons)

include(FeatureSummary)

install(DIRECTORY Crule DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/icons)
install(DIRECTORY Crule-dark DESTINATION ${CMAKE_INSTALL_PREFIX}/usr/share/icons) 
