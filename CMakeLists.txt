cmake_minimum_required(VERSION 3.6)
project(LeetCode)
set(CMAKE_CXX_STANDARD 11)

#链接库
aux_source_directory(leetcode/editor/cn/include LEETCODE)
add_library(leetcode ${LEETCODE})
LINK_LIBRARIES(leetcode)


add_executable(1-two-sum leetcode/editor/cn/1-two-sum.cpp)
add_executable(100-same-tree leetcode/editor/cn/100-same-tree.cpp)
add_executable(3-longest-substring-without-repeating-characters leetcode/editor/cn/3-longest-substring-without-repeating-characters.cpp)
add_executable(4-median-of-two-sorted-arrays leetcode/editor/cn/4-median-of-two-sorted-arrays.cpp)