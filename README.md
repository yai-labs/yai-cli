# yai-cli

`yai-cli` is the official command-line client for YAI’s control plane.
It is a thin, contract-driven interface over the pinned specs in `deps/yai-specs`.

Current release baseline: `v0.1.0`.
Current contract line: `SPECS_API_VERSION=v1`.

## What It Is

- A stable CLI surface for Root/Kernel/Engine/Mind control flows.
- A strict consumer of the CLI and protocol contracts defined in `deps/yai-specs`.
- A distribution target that produces `dist/bin/yai-cli`.

## Quickstart

Build and run the CLI locally:

```bash
make
./dist/bin/yai-cli root ping
./dist/bin/yai-cli ws list
./dist/bin/yai-cli kernel status
```

## Install

Build from source using the repo Makefile. The output binary is `dist/bin/yai-cli`.
See `docs/INSTALL.md` for prerequisites.

## Contract Discipline (Non-Negotiable)

- Canonical command set: `deps/yai-specs/specs/cli/schema/commands.v1.json`
- Canonical command schema: `deps/yai-specs/specs/cli/schema/commands.schema.json`
- Protocol envelope/IDs: `deps/yai-specs/specs/protocol/include/transport.h` and `deps/yai-specs/specs/protocol/include/yai_protocol_ids.h`

No command or protocol behavior may drift from the pinned specs.
If drift is detected, open an issue and realign before release.

## Specs Pinning

`deps/yai-specs` is an explicit pin (commit or tag), never floating.
Compatibility expectations live in `COMPATIBILITY.md`.
See `docs/SPECS_PINNING.md` for rules.

## Documentation

- `docs/COMMANDS.md` – command source of truth and schema
- `docs/CONTRACT.md` – contract boundary and canonical references
- `docs/INSTALL.md` – build/install prerequisites
- `docs/BUNDLE.md` – bundle format (if used)
- `docs/GOVERNANCE.md` – governance and change discipline
- API Reference (Doxygen): https://francescomaiomascio.github.io/yai-cli/

## Governance

- `SECURITY.md`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `CHANGELOG.md`

## Versioning

This repo follows the policy in `VERSIONING.md`.
Breaking CLI changes require a `MAJOR` bump and spec alignment.

## License

Apache License 2.0 (Apache-2.0).
The full license text is available in `LICENSE`.
Third-party licensing notices are tracked in `THIRD_PARTY_NOTICES.md`.
