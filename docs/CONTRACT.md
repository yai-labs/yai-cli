# CLI Contract Surface

## Scope

This repository provides the executable CLI interface for YAI.
It is a consumer of `yai-specs` and must stay compatible with pinned specs revisions.

## Normative Sources

Normative protocol and contract definitions are external to this repository and live in `deps/yai-specs`.
This repository must not diverge from those contracts.

## Compatibility Rules

- CLI behavior must remain compatible with the active specs major version.
- Breaking behavior changes require coordinated versioning and migration communication.
- Additive behavior should be backward compatible whenever possible.

## Non-Goals

- Defining protocol wire format in this repository.
- Duplicating canonical specs text that already exists in `yai-specs`.
