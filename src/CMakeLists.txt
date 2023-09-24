CMAKE_MINIMUM_REQUIRED(VERSION 3.12)
SET(PROJECT_NAME BBCVC2HQCBR)

PROJECT(${PROJECT_NAME})
include_directories(${PROJECT_SOURCE_DIR})
foreach(subdir 
			Library
			EncodeHQ_CBR
			DecodeHQ
		)
      add_subdirectory(${subdir})
endforeach()