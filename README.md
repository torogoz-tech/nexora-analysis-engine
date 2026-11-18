# Nexora Analysis Engine

Independent Rust packages for deterministic source analysis: language profile loading, lexing, parsing, syntax and symbol modeling, graph construction, indexing, source access, and retrieval.

Language profiles remain in their existing repositories. Database job claiming and API persistence are owned by `nexora-job-store`; this repository contains no service database credentials or queue consumers.

All packages in this repository are released together at version `0.4.0`.

## Repository status

The `0.4.0` extraction is in progress on `develop`.

## Development

Use the Rust toolchain declared by the workspace. Run `cargo fmt --all -- --check`, `cargo check --workspace --locked`, `cargo test --workspace --locked`, and `cargo clippy --workspace --all-targets --locked -- -D warnings` before submitting changes. Run the profile validation and deterministic analysis fixture commands documented in the workspace.

See [CONTRIBUTING.md](CONTRIBUTING.md), [SECURITY.md](SECURITY.md), and [CHANGELOG.md](CHANGELOG.md).
