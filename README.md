# toml.bzl

A small Bazel library which allows _repository rules_ to consume [TOML](https://toml.io/en/) files.

## Usage

Following the lead of [json](https://bazel.build/rules/lib/core/json),

``` starlark
load("@toml.bzl", "toml")

# toml.decode_file(repository_ctx, <path>)
# 
# Unsupported:
#   toml.decode(repository_ctx, <text>)
#   toml.encode_indent(repository_ctx, <obj>)
#   toml.indent(repository_ctx, <text>)
```
