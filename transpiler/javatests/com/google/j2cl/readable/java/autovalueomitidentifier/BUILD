load(
    "//transpiler/javatests/com/google/j2cl/readable:readable_example.bzl",
    "readable_example",
)

package(
    licenses = ["notice"],  # Apache 2.0
)

# Creates verification target
readable_example(
    srcs = glob(["*.java"]),
    experimental_optimize_autovalue = True,
    javacopts = ["-Acom.google.auto.value.OmitIdentifiers"],
    deps = [
        "//third_party:auto_value-j2cl",
        "//third_party:jsr305_annotations-j2cl",
    ],
)
