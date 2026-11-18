# Repository instructions

- Keep each explicit Rust type or language feature in its own focused file.
- Follow SOLID and preserve deterministic outputs across supported platforms.
- Do not introduce traits or interface abstractions unless a caller requires them.
- Keep language profiles in their existing repositories.
- Keep database connections, job stores, service secrets, and queue consumers out of this repository.
- Use `develop` for changes and pull requests to `main`.
- Keep all package versions aligned with the coordinated release version.
