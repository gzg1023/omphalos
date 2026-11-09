# Omphalos

**A local-first control center for AI agents.**

Omphalos brings tasks, runs, human approvals, and artifacts into one place, with planned support for local executors such as Claude Code and Codex.

> Early development: planning and technical validation. No runnable application or released integrations yet.

## Direction

- Submit tasks to local coding agents and follow their execution.
- Inspect persistent run events, logs, and resulting changes.
- Approve supported execution requests and review artifacts.
- Add messaging channels, memory, and durable workflows incrementally.

## First milestone

Validate one executor's structured events, permission interface, cancellation, and session recovery. Then build a single-user local Web console with a task queue, SQLite persistence, live logs, isolated Git worktrees, and result review.

Approval and recovery support will depend on verified executor capabilities. Git worktrees and subprocesses are not security sandboxes.

## Roadmap

| Stage | Focus |
| --- | --- |
| P0 | Executor capability validation and technical decisions |
| v0.1 | Local Web task lifecycle with Claude Code |
| v0.2 | Feishu channel and reliability |
| v0.3 | Codex adapter and capability mapping |
| v0.4 | Local memory and optional assistant features |
| v0.5 | Durable workflows, review, and rework |
| v1.0 | Extensions, additional channels, and release readiness |

See [the interactive development plan](docs/development-plan.html). Download the HTML and open it in a browser to track progress; progress is browser-local and can be exported as JSON.

## Planned stack

TypeScript, pnpm, React, Node.js, and SQLite. Runtime versions and integration protocols will be established during technical validation.

## Contributing

Issues and design feedback are welcome. Start with the technical validation milestone before implementing later roadmap features. Never commit credentials, private agent sessions, or personal execution logs.

## License

[Apache License 2.0](LICENSE)
