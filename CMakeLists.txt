cmake_minimum_required (VERSION 3.9)
project (cpp-jwt)

# add library target
add_library(cpp-jwt INTERFACE)

target_link_libraries(cpp-jwt
	INTERFACE
	ssl
	crypto
	tls
)

# list include directories
target_include_directories(cpp-jwt
	INTERFACE
	${CMAKE_CURRENT_SOURCE_DIR}/include
)