set(target postfix_test)

#file(GLOB hdrs "*.h*" "../include/*.h" "../gtest/*.h")
file(GLOB hdrs "*.h*")
file(GLOB srcs "*.cpp" "../src/postfix.cpp")

add_executable(${target} ${srcs} ${hdrs})
target_link_libraries(${target} gtest)