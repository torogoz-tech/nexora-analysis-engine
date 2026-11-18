# Nexora Analysis Engine

Independent Rust packages for deterministic source analysis: language profile loading, lexing, parsing, syntax and symbol modeling, graph construction, indexing, source access, and retrieval.

Language profiles remain in their existing repositories. The root `languages/` and `templates/` directories are regression fixtures used by integration tests; they are not the source of published language profiles. Database job claiming and API persistence are owned by `nexora-job-store`; this repository contains no service database credentials or queue consumers.

The packages in this workspace are released together at version `0.4.0`.

## Development

Use the Rust toolchain declared by the workspace. Before submitting changes, run `cargo fmt --all -- --check`, `cargo check --workspace --locked`, `cargo test --workspace --locked`, and `cargo clippy --workspace --all-targets --locked -- -D warnings`. The package integration tests validate deterministic analysis behavior against the checked-in fixtures under `languages/`, `templates/`, `corpus/`, and `tests/fixtures/`.

See [CONTRIBUTING.md](CONTRIBUTING.md), [SECURITY.md](SECURITY.md), and [CHANGELOG.md](CHANGELOG.md).
