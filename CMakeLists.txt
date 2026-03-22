cmake_minimum_required(VERSION 3.10)
project(kmz80 VERSION 1.0.0 LANGUAGES C)

add_library(kmz80 STATIC
  kmdmg.c
  kmevent.c
  kmr800.c
  kmz80.c
  kmz80c.c
  kmz80t.c
)

target_include_directories(kmz80 PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

set_target_properties(kmz80 PROPERTIES
  C_STANDARD 99
  C_STANDARD_REQUIRED ON
)

target_compile_options(kmz80 PRIVATE
  $<$<C_COMPILER_ID:MSVC>:/W3 /WX /utf-8 /wd4996>
  $<$<NOT:$<C_COMPILER_ID:MSVC>>:-Wall -Werror>
)
