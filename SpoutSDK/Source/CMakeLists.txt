cmake_minimum_required(VERSION 3.11)
project(spout2 VERSION 2.006 LANGUAGES CXX)

add_library(spout2
			STATIC
			SpoutCopy.cpp
			SpoutDirectX.cpp
			SpoutGLDXinterop.cpp
			SpoutGLextensions.cpp
			SpoutMemoryShare.cpp
			SpoutReceiver.cpp
			SpoutSDK.cpp
			SpoutSender.cpp
			SpoutSenderMemory.cpp
			SpoutSenderNames.cpp
			SpoutSharedMemory.cpp)

target_include_directories(spout2 
		                   PUBLIC
						   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(spout2 PROPERTIES VERSION ${PROJECT_VERSION})

