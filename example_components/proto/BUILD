load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_cc//cc:defs.bzl", "cc_proto_library")
load("//tools:python_rules.bzl", "py_proto_library")
load("//tools/install:install.bzl", "install", "install_files")

package(default_visibility = ["//visibility:public"])

cc_proto_library(
    name = "examples_cc_proto",
    deps = [
        ":examples_proto",
    ],
)

proto_library(
    name = "examples_proto",
    srcs = ["examples.proto"],
)

py_proto_library(
    name = "examples_py_pb2",
    deps = [
        ":examples_proto",
    ],
)
