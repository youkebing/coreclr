cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test13.c
)

add_executable(paltest_snwprintf_test13
  ${SOURCES}
)

add_dependencies(paltest_snwprintf_test13 CoreClrPal)

target_link_libraries(paltest_snwprintf_test13
  pthread
  rt
  m
  CoreClrPal
)
