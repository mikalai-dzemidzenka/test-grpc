load("@bazel_gazelle//:def.bzl", "gazelle", "DEFAULT_LANGUAGES", "gazelle_binary")

gazelle_binary(
    name = "gazelle_binary",
    languages = DEFAULT_LANGUAGES + ["@golink//gazelle/go_link:go_default_library"],
    visibility = ["//visibility:public"],
)

# gazelle:prefix test-grpc
gazelle(
    name = "gazelle",
    gazelle = "//:gazelle_binary",
)
