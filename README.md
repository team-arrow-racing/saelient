# Saelient: SAE-J1939 in Rust

Saelient provides a helper interface on top of [`embedded_can`](https://crates.io/crates/embedded-can) traits compatible with `no-std` targets.

## Getting Started

Run the following Cargo command in your project directory:

```shell
cargo add saelient
```

## Principles

- Zero-copy wherever possible by creating views on data rather than mutating or copying.
- Easily understandable API. You shouldn't need to read the whole J1939 spec to understand how the API works.
- Lightweight. Should not bloat binary sizes with inefficient concepts like error strings that would usually be accepted in non `no-std` environments.
