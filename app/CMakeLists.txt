file(GLOB_RECURSE srcs CONFIGURE_DEPENDS src/*.cpp include/*.h)
add_executable(app ${srcs})
target_link_libraries(app PUBLIC glfw)
target_link_libraries(app PUBLIC imgui)
target_link_libraries(app PUBLIC opengl32)

target_include_directories(app PUBLIC include)
