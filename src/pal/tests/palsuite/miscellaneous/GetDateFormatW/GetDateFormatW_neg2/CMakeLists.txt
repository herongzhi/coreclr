cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  GetDateFormatW_neg.c
)

add_executable(paltest_getdateformatw_getdateformatw_neg2
  ${SOURCES}
)

add_dependencies(paltest_getdateformatw_getdateformatw_neg2 CoreClrPal)

target_link_libraries(paltest_getdateformatw_getdateformatw_neg2
  pthread
  rt
  m
  CoreClrPal
)
