```
$ bazel build //:gen_rust_project
INFO: Repository rules_rust~0.35.0~rust~rust_darwin_aarch64__aarch64-apple-darwin__stable_tools instantiated at:
  <builtin>: in <toplevel>
Repository rule rust_toolchain_tools_repository defined at:
  /private/var/tmp/<snip>/external/rules_rust~0.35.0/rust/repositories.bzl:373:50: in <toplevel>
ERROR: no such package '@@[unknown repo 'rust_analyzer_1.74.0_srcs' requested from @@rules_rust~0.35.0~rust~rust_toolchains]//': The repository '@@[unknown repo 'rust_analyzer_1.74.0_srcs' requested from @@rules_rust~0.35.0~rust~rust_toolchains]' could not be resolved: No repository visible as '@rust_analyzer_1.74.0_srcs' from repository '@@rules_rust~0.35.0~rust~rust_toolchains'
ERROR: /private/var/tmp/<snip>/external/rules_rust~0.35.0/rust/private/BUILD.bazel:33:29: Target '@@rules_rust~0.35.0//rust/private:rust_analyzer_detect_sysroot' depends on toolchain '@@[unknown repo 'rust_analyzer_1.74.0_srcs' requested from @@rules_rust~0.35.0~rust~rust_toolchains]//:rust_analyzer_toolchain', which cannot be found: no such package '@@[unknown repo 'rust_analyzer_1.74.0_srcs' requested from @@rules_rust~0.35.0~rust~rust_toolchains]//': The repository '@@[unknown repo 'rust_analyzer_1.74.0_srcs' requested from @@rules_rust~0.35.0~rust~rust_toolchains]' could not be resolved: No repository visible as '@rust_analyzer_1.74.0_srcs' from repository '@@rules_rust~0.35.0~rust~rust_toolchains''
ERROR: Analysis of target '//:gen_rust_project' failed; build aborted: Analysis failed
INFO: Elapsed time: 0.501s, Critical Path: 0.00s
INFO: 1 process: 1 internal.
ERROR: Build did NOT complete successfully
FAILED:
    Fetching repository @@bazel_tools~cc_configure_extension~local_config_cc; starting
```
