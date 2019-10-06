cmake_minimum_required(VERSION 3.6)

include(cmake/cppm_tool.cmake)
cppm_project()
project(md5 VERSION 0.0.1 LANGUAGES C CXX)
cppm_setting()

cppm_cxx_standard(17)
cppm_compiler_option(DEFAULT)



cppm_target_define(md5 STATIC 
SOURCES 
	src/md5.cpp)


cppm_target_dependencies(md5 
)

cppm_target_install(md5)

