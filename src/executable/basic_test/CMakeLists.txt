find_package(Threads)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

add_executable(basic_test main.cpp)

target_link_libraries(basic_test 
PRIVATE
    ${CMAKE_THREAD_LIBS_INIT} 
    work_contract
)