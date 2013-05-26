# Copyright (c) 2013 Plenluno All rights reserved.

cmake_minimum_required(VERSION 2.8)

project(googletest)

include_directories(
    include
)

add_library(gtest STATIC
    src/gtest-all.cc
)

set_target_properties(gtest PROPERTIES
    COMPILE_FLAGS "${libj-test-cflags}"
)
