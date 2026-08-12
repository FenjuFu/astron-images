# Astron Agent × dolphin-mcp-pilot real-run screenshots

These images document an isolated local run of Astron Agent v1.1.1, dolphin-mcp-pilot v0.3.0, and Apache DolphinScheduler 3.2.2.

The sequence covers repository/version identification, Astron ReACT MCP configuration, real MCP tool calls, a controlled FAILURE, the static `next_action` hint, failed-task log inspection, one accepted rerun-from-failure request, continued polling, and the final DolphinScheduler SUCCESS state.

Important boundaries:

- `next_action` is a code-generated static hint, not model diagnosis.
- `submitted` means the rerun request was accepted; it is not proof of recovery.
- Recovery is claimed only after the real scheduler state reaches `SUCCESS`.
- These are isolated test-environment captures, not a production deployment.
- No credentials, passwords, tokens, cookies, or API secrets appear in the images.

Sources:

- https://github.com/iflytek/dolphin-mcp-pilot
- https://github.com/iflytek/astron-agent
- https://github.com/apache/dolphinscheduler
