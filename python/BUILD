package(default_visibility = ["//visibility:public"])

py_library(
    name = "hardware_abstraction",
    srcs = ["hardware_abstraction.py"],
)

py_library(
    name = "commlink",
    srcs = ["commlink.py"],
    deps = [
        ":hardware_abstraction",
    ],
)

py_test(
    name = "hardware_abstraction_test",
    srcs = ["hardware_abstraction_test.py"],
    deps = [":hardware_abstraction"],
)

py_test(
    name = "packet_test",
    srcs = ["packet_test.py"],
    deps = [":commlink",
            ":hardware_abstraction"],
)

py_test(
    name = "commlink_writer_test",
    srcs = ["commlink_writer_test.py"],
    deps = [":commlink",
            ":hardware_abstraction"],
)

py_test(
    name = "commlink_reader_test",
    srcs = ["commlink_reader_test.py"],
    deps = [":commlink",
            ":hardware_abstraction"],
)

py_test(
    name = "commlink_test",
    srcs = ["commlink_test.py"],
    deps = [":commlink",
            ":hardware_abstraction"],
    timeout = "short",
)

py_test(
    name = "commlink_fault_test",
    srcs = ["commlink_fault_test.py"],
    deps = [":commlink",
            ":hardware_abstraction"],
    timeout = "eternal",
)

py_test(
    name = "commlink_profile",
    srcs = ["commlink_profile.py"],
    deps = [":commlink",
            ":hardware_abstraction"],
)
