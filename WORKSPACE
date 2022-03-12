load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "d6b2513456fe2229811da7eb67a444be7785f5323c6708b38d851d2b51e54d83",
    urls = [
        "https://mirror.bazel.build/github.com/bazelbuild/rules_go/releases/download/v0.30.0/rules_go-v0.30.0.zip",
        "https://github.com/bazelbuild/rules_go/releases/download/v0.30.0/rules_go-v0.30.0.zip",
    ],
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "e9c02f13706e8b1ef05b57e6ae4d59910643bebac6d4e82581aa8c75fce6998b",
    strip_prefix = "bazel-gazelle-e21487a75fffa5616846e3c69de16f65c8953bad",
    urls = [
        "https://github.com/bazelbuild/bazel-gazelle/archive/e21487a75fffa5616846e3c69de16f65c8953bad.tar.gz",
        "https://mirror.bazel.build/github.com/bazelbuild/bazel-gazelle/archive/e21487a75fffa5616846e3c69de16f65c8953bad.tar.gz",
    ],
)

load("@io_bazel_rules_go//go:deps.bzl", "go_register_toolchains", "go_rules_dependencies")
load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")

go_rules_dependencies()

go_register_toolchains(version = "1.17.6")

gazelle_dependencies()
