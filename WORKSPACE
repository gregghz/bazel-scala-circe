rules_scala_version="85308acbd316477f3072e033e7744debcba4f054" # update this as needed

http_archive(
  name = "io_bazel_rules_scala",
  url = "https://github.com/bazelbuild/rules_scala/archive/%s.zip"%rules_scala_version,
  type = "zip",
  strip_prefix= "rules_scala-%s" % rules_scala_version
)

load("@io_bazel_rules_scala//scala:scala.bzl", "scala_repositories")
scala_repositories()

maven_jar(
  name = "org_scalamacros_paradise_2_11_11",
  artifact = "org.scalamacros:paradise_2.11.11:2.1.0",
)

circeVersion = "0.9.0-M1"

maven_jar(
 name = "io_circe_circe_core",
 artifact = "io.circe:circe-core_2.11:{}".format(circeVersion),
)

maven_jar(
 name = "io_circe_circe_literal",
 artifact = "io.circe:circe-literal_2.11:{}".format(circeVersion),
)

maven_jar(
 name = "io_circe_circe_parser",
 artifact = "io.circe:circe-parser_2.11:{}".format(circeVersion),
)

maven_jar(
 name = "io_circe_circe_jawn",
 artifact = "io.circe:circe-jawn_2.11:{}".format(circeVersion),
)
