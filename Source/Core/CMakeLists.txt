set(TARGET_NAME Core)

file(GLOB_RECURSE h_files "*.h")
file(GLOB_RECURSE cpp_files "*.cpp")
add_library (${TARGET_NAME} ${h_files} ${cpp_files})


target_include_directories(${TARGET_NAME} PUBLIC ${THIRD_PARTY}/glm)