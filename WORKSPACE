workspace(name = "bazel_remote_apis")

load("//bazel:remote_apis_deps.bzl", "remote_apis_deps")

remote_apis_deps()

# Pull in all gRPC dependencies.
load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")
grpc_deps()

load("@io_bazel_rules_go//go:deps.bzl", "go_rules_dependencies", "go_register_toolchains")
go_rules_dependencies()
go_register_toolchains()
