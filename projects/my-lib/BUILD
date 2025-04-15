load("@rules_angular//src/architect:ng_library.bzl", "ng_library")
load("@rules_angular//src/architect:ng_test.bzl", "ng_test")

package(default_visibility = ["//visibility:public"])

ng_library(
    name = "my-lib",
    ng_config = "//:ng-config",
    node_modules = "//:node_modules",
)

ng_test(
    name = "test",
    ng_config = "//:ng-config",
    node_modules = "//:node_modules",
    tags = ["no-sandbox"],
)
