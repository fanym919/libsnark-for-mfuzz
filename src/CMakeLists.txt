include_directories(.)

add_executable(
  test

  test.cpp
)
target_link_libraries(
  test

  snark
)
target_include_directories(
  test

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
)

include_directories(.)

add_executable(
  range

  range.cpp
)
target_link_libraries(
  range

  snark
)
target_include_directories(
  range

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
)

include_directories(.)

add_executable(
  groth16

  groth16.cpp
)
target_link_libraries(
  groth16

  snark
)
target_include_directories(
  groth16

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
)
