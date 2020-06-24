cmake_minimum_required( VERSION 3.6 )
project( Houdini_Minimal_Plugin )

#list( APPEND CMAKE_PREFIX_PATH "$ENV{HFS}/toolkit/cmake" )
list( APPEND CMAKE_PREFIX_PATH "D:/Program Files/Side Effects Software/Houdini 18.0.499/toolkit/cmake" )
find_package( Houdini REQUIRED )

set( library_name Minimal_Plugin )
add_library(${library_name} SHARED
	Minimal_Plugin.C
)

target_link_libraries( ${library_name} Houdini )

# Configure several common target properties, such as its output directory.
houdini_configure_target( ${library_name} )
