add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/thirdparty/SQLiteCpp)

add_executable(main src/main.cpp)
target_link_libraries(main
  SQLiteCpp
  sqlite3
  pthread
  dl
  )