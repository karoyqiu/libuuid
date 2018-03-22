cmake_minimum_required(VERSION 3.8)

project(uuid C)

add_library(uuid STATIC
	clear.c
	compare.c
	copy.c
	gen_uuid.c
	isnull.c
	pack.c
	parse.c
	unpack.c
	unparse.c
	uuidd.h
	uuidP.h
	uuid_time.c
	randutils.c
	all-io.h
	c.h
	randutils.h
	uuid.h
)
target_include_directories(uuid INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}")
