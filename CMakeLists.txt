cmake_minimum_required(VERSION 3.0.0)

project(xgetopt VERSION 1.0.0)

install(DIRECTORY "./" # source directory
        DESTINATION "include" # target directory
        #FILES_MATCHING # install only matched files
        #PATTERN "*.h;*.cpp" # select header files
)