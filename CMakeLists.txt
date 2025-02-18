cmake_minimum_required(VERSION 3.16)
project(lf_queue)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)


set(LF_QUEUE_SOURCES
  ${CMAKE_CURRENT_SOURCE_DIR}/src/lf_queue.c
  ${CMAKE_CURRENT_SOURCE_DIR}/src/lf_misc.h
  ${CMAKE_CURRENT_SOURCE_DIR}/include/lf_queue.h
)

add_library(lf_queue)
target_sources(lf_queue
 PRIVATE
  ${LF_QUEUE_SOURCES}
  )

target_include_directories(lf_queue
 PRIVATE
 include
 )
