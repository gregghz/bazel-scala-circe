load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library")

scala_library(
  name = "sample",
  srcs = glob(["src/**/*.scala"]),
  visibility = ["//visibility:public"],
  plugins = ["@org_scalamacros_paradise_2_11_11//jar"],
  deps = [
    "@io_circe_circe_core//jar",
    "@io_circe_circe_literal//jar:file",
    "@io_circe_circe_parser//jar",
    "@io_circe_circe_jawn//jar",
  ]
)