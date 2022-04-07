load("@local_config_platform//:constraints.bzl", "HOST_CONSTRAINTS")

platform(
    name = "host",
    constraint_values = HOST_CONSTRAINTS + [
        "//cxx:20",
        "//cxx:hosted",
    ],
)

platform(
    name = "rpi3",
    constraint_values = [
        "@platforms//os:none",
        "//cpu:cortex-a53-nosimd",
        "//cxx:20",
        "//cxx:freestanding",
    ],
    target_platform = True,
)

platform(
    name = "pico",
    constraint_values = [
        "@platforms//os:none",
        "@platforms//cpu:armv6-m",
        "//cxx:20",
    ],
    target_platform = True,
)
