load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["reference.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/go-openapi/jsonreference",
    importpath = "github.com/go-openapi/jsonreference",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/PuerkitoBio/purell:go_default_library",
        "//vendor/github.com/go-openapi/jsonpointer:go_default_library",
    ],
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
