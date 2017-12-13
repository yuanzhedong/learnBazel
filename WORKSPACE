workspace(name = "qap")
#load("//protobuf:rules.bzl", "github_archive")
git_repository(
    name = "org_pubref_rules_protobuf",
    remote = "https://github.com/pubref/rules_protobuf.git",
    tag = "v0.8.1",
    # commit doesn't work
    #commit = "4af9492303698b9efe46053b74c7a55a16c49085",
)

# new_http_archive(
#     name = "gtest",
#     url = "https://github.com/google/googletest/archive/release-1.7.0.zip",
#     sha256 = "b58cb7547a28b2c718d1e38aee18a3659c9e3ff52440297e965f5edffe34b6d0",
#     build_file = "gtest.BUILD",
#     strip_prefix = "googletest-release-1.7.0",
# )

#load("@org_pubref_rules_protobuf//protobuf:rules.bzl", "proto_repositories")
#proto_repositories()

# Load language-specific dependencies
load("@org_pubref_rules_protobuf//cpp:rules.bzl", "cpp_proto_repositories")
# this is a function defined in cpp:rules.bzl, will load third party libraies like @com_google_googletest
# and define alias like
# Alias for cpp_proto_library
# cc_proto_library = cpp_proto_library
cpp_proto_repositories()