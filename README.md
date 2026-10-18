# margo-gateway

A multi-provider AI gateway, written in Go, that fronts the models
[Margo](https://github.com/kumouri/seneschal) (Ceryce's chief-of-staff assistant) calls every day:
Claude (CLI), Codex, Antigravity, and OpenRouter. It handles routing, budgets, retries and per-call
logging behind one HTTP API.

It is also how I'm learning Go. Each milestone teaches one part of the language and ships something
that runs in production.

## Milestones

| # | Builds | Go it teaches | Status |
|---|---|---|---|
| 0 | `hello` service + a test; module and repo layout | modules, packages, `go test` | ☐ |
| 1 | HTTP endpoint: prompt in, JSON out | `net/http`, structs, JSON tags, errors as values | ☐ |
| 2 | Call `claude -p` from the service, with a timeout | `os/exec`, `context`, cancellation | ☐ |
| 3 | Claude, Codex, Antigravity and OpenRouter behind one interface | interfaces, HTTP client | ☐ |
| 4 | Concurrency limits; retries with backoff | goroutines, channels, `sync` | ☐ |
| 5 | Per-route budgets; a log of every call and its cost | persistence, `log/slog` | ☐ |
| 6 | CI, a release, docs | GitHub Actions for Go, `go vet`, linting | ☐ |
| 7 | Margo routes her real calls through it | running it for real | ☐ |

## License

Apache-2.0
