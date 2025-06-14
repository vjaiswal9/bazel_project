cc_library(
    name = "helper_lib",
    srcs = ["helper.cpp"],
    hdrs = ["helper.h"],
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "main_cpp",
    srcs = ["main.cpp"],
    deps = [":helper_lib"],
    data = ["//data:config_data"],
)

py_binary(
    name = "main_py",
    srcs = ["main.py"],
    deps = [],
)

