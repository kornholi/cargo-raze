"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = [
  # Public for visibility by "@raze__crate__version//" targets.
  #
  # Prefer access through "//vendored/non_cratesio_library/cargo", which limits external
  # visibility to explicit Cargo.toml dependencies.
  "//visibility:public",
])

licenses([
  "notice", # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
)


# Unsupported target "channel" with type "test" omitted

rust_library(
    name = "futures_channel",
    crate_root = "src/lib.rs",
    crate_type = "lib",
    srcs = glob(["**/*.rs"]),
    deps = [
        "//vendored/non_cratesio_library/cargo/vendor/futures-core-0.2.0-alpha:futures_core",
    ],
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.2.0-alpha",
    crate_features = [
        "futures-core",
        "std",
    ],
)

# Unsupported target "mpsc" with type "test" omitted
# Unsupported target "mpsc-close" with type "test" omitted
# Unsupported target "oneshot" with type "test" omitted
# Unsupported target "sync_mpsc" with type "bench" omitted
