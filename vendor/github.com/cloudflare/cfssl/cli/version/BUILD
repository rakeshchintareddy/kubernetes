load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "version.go",
        "version_dev.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/github.com/cloudflare/cfssl/cli/version",
    importpath = "github.com/cloudflare/cfssl/cli/version",
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/cloudflare/cfssl/cli:go_default_library"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
