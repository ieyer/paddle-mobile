
# gen test
ADD_EXECUTABLE(test-conv-op  operators/test_cov_op.cpp test_helper.h  test_include.h)
target_link_libraries(test-conv-op paddle-mobile)

# gen test
ADD_EXECUTABLE(test-mul-op  operators/test_mul_op.cpp test_helper.h  test_include.h)
target_link_libraries(test-mul-op paddle-mobile)

# gen test
ADD_EXECUTABLE(test-elementwiseadd-op  operators/test_elementwise_add_op.cpp test_helper.h  test_include.h)
target_link_libraries(test-elementwiseadd-op paddle-mobile)


# gen test log
ADD_EXECUTABLE(test-log common/test_log.cpp)
target_link_libraries(test-log paddle-mobile)

# gen test log
ADD_EXECUTABLE(test-load framework/test_load.cpp)
target_link_libraries(test-load paddle-mobile)


# gen test log
ADD_EXECUTABLE(test-optimize framework/test_optimize.cpp)
target_link_libraries(test-optimize paddle-mobile)