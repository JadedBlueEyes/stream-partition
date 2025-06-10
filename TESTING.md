
# Memory leaks

<https://doc.rust-lang.org/beta/unstable-book/compiler-flags/sanitizer.html#addresssanitizer>

```sh
export RUSTFLAGS=-Zsanitizer=address RUSTDOCFLAGS=-Zsanitizer=address ASAN_OPTIONS=detect_leaks=1
cargo +nightly -Zbuild-std test --target <your-target>
```

A baseline amount of leak is expected to be detected - for `rustc 1.88.0-nightly (d6a325d93 2025-05-03)` that's around 704 bytes. Run test_memory_usage with increasing iterations and test that that stays the same.

Not sure how to automate this, though.
