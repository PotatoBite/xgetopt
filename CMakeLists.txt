cmake_minimum_required(VERSION 3.0.0)

project(xgetopt VERSION 1.0.0)

ADD_LIBRARY( xgetopt STATIC xgetopt.c )
			 
install(DIRECTORY "./" # source directory
        DESTINATION "include" # target directory
        FILES_MATCHING # install only matched files
        PATTERN "*.h" # select header files
		PATTERN "*.c" # select header files
		PATTERN "*.cpp" # select header files
)

install(TARGETS xgetopt # source directory
        DESTINATION "lib" # target directory
)