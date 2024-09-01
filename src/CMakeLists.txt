#
# Set up our executable
add_executable(${PROJECT_NAME_SNAKE}
    "${PROJECT_NAME_SNAKE}.cpp"
 )

#
# Set output directory
set_target_properties(${PROJECT_NAME_SNAKE} PROPERTIES
    CXX_STANDARD             20
    CXX_STANDARD_REQUIRED    TRUE
    RUNTIME_OUTPUT_DIRECTORY $${${PROJECT_NAME_DEFINE}_OUTPUT_PATH})

# Set target includes
target_include_directories(${PROJECT_NAME_SNAKE}
    PRIVATE $${CMAKE_SOURCE_DIR}/include
    PUBLIC  $${CMAKE_SOURCE_DIR}/include)
