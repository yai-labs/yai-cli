# YAI CLI

Canonical command-line entrypoint for YAI runtime operations.
This repository is the public CLI surface consumed by operators, scripts, and higher-level tools.

## What This Repo Provides

- CLI binary build and distribution (`yai-cli`)
- Stable command routing to runtime planes (`root`, `kernel`, `engine`, `mind`)
- Contract-aligned integration with pinned `yai-specs`

## Public Contract Boundary

Normative compatibility is defined by pinned specs in `deps/yai-specs`.
Implementation lives in this repository, while protocol/contract truth lives in specs.

## Install

Build from source using the project Makefile.
The binary is produced under `dist/bin/yai-cli`.

## Usage

Use `yai-cli` as the operator entrypoint for runtime control commands.
Command behavior must remain aligned with active specs and compatibility rules.

## Bundle / Pinning Model

Consumers should treat this CLI as part of a pinned stack:
- pin `yai-cli` revision
- pin compatible `yai-specs` revision
- upgrade both deliberately, validating compatibility before rollout

## Repository Governance

- `CONTRIBUTING.md` for contribution rules
- `SECURITY.md` for security reporting
- `CODE_OF_CONDUCT.md` for collaboration standards
- `docs/` for contract and operational documentation
