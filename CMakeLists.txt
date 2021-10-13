file(GLOB_RECURSE SOURCE_FILES
    src/*.cpp
    include/*.h
)

add_library(yamlcpp ${SOURCE_FILES})

target_include_directories(yamlcpp PRIVATE include)

set_target_properties(yamlcpp PROPERTIES FOLDER dependencies)
