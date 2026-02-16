# Contract Boundary

`yai-cli` implementa e consuma specs pin-nate in `deps/yai-specs`.
Le specs in quella directory sono la source-of-truth contrattuale.

## Canonical References

- Commands contract: `deps/yai-specs/cli/commands.v1.json`
- Commands schema: `deps/yai-specs/cli/commands.schema.json`
- Protocol envelope/IDs: `deps/yai-specs/protocol/transport.h`, `deps/yai-specs/protocol/yai_protocol_ids.h`
- Errors/auth/roles: `deps/yai-specs/protocol/errors.h`, `deps/yai-specs/protocol/auth.h`, `deps/yai-specs/protocol/roles.h`

## Rule

Nessuna semantica comando/protocollo puo' essere inventata fuori dalle specs pin-nate.
Se c'e' drift: aprire issue e riallineare CLI/specs prima del rilascio.
