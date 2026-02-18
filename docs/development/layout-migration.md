# Layout Migration Mapping

| OLD_PATH | NEW_PATH | TYPE | NOTES |
|---|---|---|---|
| include/yai_cli.h | include/yai_cli/cli.h | header | Namespaced public header |
| include/yai_cmd.h | include/yai_cli/cmd.h | header | Namespaced public header |
| include/yai_cmd_law.h | include/yai_cli/cmd_law.h | header | Namespaced public header |
| include/yai_env.h | include/yai_cli/env.h | header | Namespaced public header |
| include/yai_fmt.h | include/yai_cli/fmt.h | header | Namespaced public header |
| include/yai_paths.h | include/yai_cli/paths.h | header | Namespaced public header |
| include/yai_rpc.h | include/yai_cli/rpc.h | header | Namespaced public header |
| src/main.c | src/main.c | src | Entry point unchanged |
| src/cmd_dispatch.c | src/cli/dispatch.c | src | CLI dispatch module |
| src/env.c | src/platform/env.c | src | Platform environment support |
| src/paths.c | src/platform/paths.c | src | Platform paths support |
| src/fmt.c | src/support/fmt.c | src | Support formatting module |
| src/rpc.c | src/runtime/rpc_client.c | src | Runtime RPC client module |
| src/cmd_root.c | src/commands/root.c | src | Command module |
| src/cmd_kernel.c | src/commands/kernel.c | src | Command module |
| src/cmd_engine.c | src/commands/engine.c | src | Command module |
| src/cmd_ws.c | src/commands/workspace.c | src | Command module |
| src/cmd_up.c | src/commands/up.c | src | Command module |
| src/cmd_law.c | src/commands/law.c | src | Command module |
| src/cmd_mind.c | src/commands/mind.c | src | Command module |
| src/cmd_test.c | src/commands/selftest.c | src | Command module (name retained in behavior) |
| docs/INSTALL.md | docs/guide/install.md | doc | Guide content re-homed |
| docs/COMMANDS.md | docs/guide/commands.md | doc | Guide content re-homed |
| docs/CONTRACT.md | docs/reference/contract.md | doc | Reference content re-homed |
| docs/GOVERNANCE.md | docs/reference/governance.md | doc | Reference content re-homed |
| docs/BUNDLE.md | docs/reference/bundle.md | doc | Reference content re-homed |
| docs/SPECS_PINNING.md | docs/development/specs-pinning.md | doc | Development reference re-homed |
| docs/api/C_MAINPAGE.md | docs/api/C_MAINPAGE.md | doc | Path unchanged |
| docs/README.md | docs/README.md | doc | Path unchanged |
| scripts (legacy) release/bump_version.sh | tools/release/bump_version.sh | tool | Removed from scripts directory |
| tests/test_parse.c | tests/unit/parse_test.c | test | Unit test path normalized |
| tests/test_rpc_vectors.c | tests/vectors/rpc_vectors_test.c | test | Vectors test path normalized |
| tests/README.md | tests/README.md | test | Path unchanged |

## Verification Log

Pending.
