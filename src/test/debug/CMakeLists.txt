get_filename_component(p ${CMAKE_CURRENT_SOURCE_DIR} NAME)
set(EXE t.${p})
add_executable(${EXE} main.cpp)
target_link_libraries(${EXE} mesh suspender)
add_test_current(COMMAND test)

