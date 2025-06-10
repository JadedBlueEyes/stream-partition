
# stream-partition

[![CI status](https://github.com/JadedBlueEyes/stream-partition/actions/workflows/rust-checks.yml/badge.svg?branch=main)](https://github.com/JadedBlueEyes/stream-partition/actions/workflows/ci.yml?query=branch%3Amain) [![dependency status](https://deps.rs/repo/github/JadedBlueEyes/stream-partition/status.svg?path=crates%2Fmrmx)](https://deps.rs/repo/github/JadedBlueEyes/stream-partition?path=crates%2Fmrmx) [![Last commit](https://img.shields.io/github/last-commit/JadedBlueEyes/stream-partition.svg?logo=github&logoColor=white)](https://github.com/JadedBlueEyes/stream-partition/commits/main/)

A Rust library for partitioning a single stream into multiple sub-streams based on keys.

## Overview

`stream-partition` provides a utility to split a stream into multiple sub-streams, where each sub-stream contains only items that match a specific key determined by an async function.

This can be used to process different types of items from a single stream with different logic.
