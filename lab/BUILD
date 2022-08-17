load("@pip//:requirements.bzl", "requirement")
load("@swift-jupyter//:lab.bzl", "jupyterlab")

py_library(
    name = "common",
    visibility = ["//lab:__subpackages__"],
    deps = [
        requirement("jupyterlab"),
        requirement("pandas"),
        requirement("numpy"),
        requirement("psycopg2"),
        requirement("matplotlib"),
        requirement("sqlalchemy"),
        requirement("xlrd"),
    ],
)

jupyterlab(
    name = "bootup",
    deps = [":common"],
)
