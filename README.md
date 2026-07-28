# Hi, I'm Maksim Martianov

Software Engineer in Security at Snowflake | Ex-Twitter, Route4Me, and others

Currently building **GALA** -- a functional programming language that transpiles to Go.

## Links

- Blog: [martianov.dev](https://martianov.dev)
- GALA: [gala.fyi](https://gala.fyi)
- Playground: [gala-playground.fly.dev](https://gala-playground.fly.dev)

## My Projects

| Project | Description |
|---------|-------------|
| [**gala**](https://github.com/martianoff/gala) | GALA programming language -- sealed types, exhaustive pattern matching, `bind`/`also` do-notation, and compile-time data-race safety. 123 releases, 388 tests. |
| [**rules-gala**](https://github.com/martianoff/rules-gala) | Bazel rules, a bzlmod extension, and a gazelle plugin for building, testing, and transpiling GALA -- also a Bazel module registry that publishes `rules_gala`. |
| [**gala-playground**](https://github.com/martianoff/gala-playground) | Web-based GALA editor with live transpilation -- 15 built-in examples, instant compilation, error display. Try it at [gala-playground.fly.dev](https://gala-playground.fly.dev). |
| [**gala-server**](https://github.com/martianoff/gala-server) | Immutable HTTP server library -- builder pattern, 35+ composable filters (auth, CORS, rate limiting, circuit breaker), SSE, zero-reflection JSON, graceful shutdown. Inspired by Finagle + Echo. |
| [**gala-tui**](https://github.com/martianoff/gala-tui) | Functional, Elm-architecture TUI framework written in GALA -- immutable widgets, differential renderer, async runtime, mouse, markdown, themes. |
| [**gala-team**](https://github.com/martianoff/gala-team) | Multi-agent Claude CLI orchestrator -- a Team Lead delegates to Engineers and QAs, reviews work, hands you a PR for sign-off. Written in GALA with gala_tui. |
| [**gala-acp**](https://github.com/martianoff/gala-acp) | Transport-neutral Agent Communication Protocol -- content-hash message identity, idempotent dedup, a delivery/liveness FSM, and a generic agent-run contract, with a Claude backend. Shared by gala-team and gala-assimilator. |
| [**gala-assimilator**](https://github.com/martianoff/gala-assimilator) 🚧 | **Under construction.** Terminal UI that migrates a codebase between languages by orchestrating AI agents in a translate -> verify -> fix loop, per file, until 100% migrated. Semantics-preserving: a unit is Done only when its 1:1 source tests pass. First pair: Go -> GALA. Written in GALA with gala_tui. |
| [**gala-state-machine-example**](https://github.com/martianoff/gala-state-machine-example) | State machines with sealed types and pattern matching -- order FSM, traffic light, vending machine. The compiler guarantees every transition is handled. Side-by-side Go comparison included. |
| [**gala-log-analyzer**](https://github.com/martianoff/gala-log-analyzer) | Structured log parsing -- demonstrates Go stdlib interop (strings, strconv, fmt) with functional pipelines (FoldLeft, Filter, HashMap aggregation). Side-by-side Go comparison included. |

## Blog

### GALA From the Ground Up

- [Data Races Are a Compile Error Now: GALA in July (0.63 -> 0.72)](https://martianov.dev/gala-july-2026-data-race-safety)
- [GALA in June: do-notation, applicative validation, and concurrent binds (0.56 -> 0.62)](https://martianov.dev/gala-june-2026-bind-also)
- [From Zero to a Go Module on Bazel in One Sitting: Onboarding to GALA 0.53](https://martianov.dev/from-zero-to-a-go-module-on-bazel-onboarding-gala-053)
- [Productionizing the GALA Build Stack: rules_gala, a Real Toolchain, and Gazelle](https://martianov.dev/productionizing-the-gala-build-stack-rules-gala-toolchain-gazelle)
- [The State of GALA: May 2026](https://martianov.dev/state-of-gala-may-2026)
- [The State of GALA: March 2026](https://martianov.dev/state-of-gala-march-2026)

### Compilers and tooling

- [Splitting the Brain: Plugin vs LSP](https://martianov.dev/splitting-the-brain-plugin-vs-lsp)
- [Dot Completion Without a Type Checker](https://martianov.dev/dot-completion-without-a-type-checker)
- [The Type Information Problem](https://martianov.dev/lsp-type-information-problem)
- [22x Faster Builds: Inside GALA's Compilation Performance Journey](https://martianov.dev/22x-faster-builds-gala-compilation-performance)
- [Building a Reliable Transpiler: Lessons from 80+ Bug Fixes](https://martianov.dev/building-reliable-transpiler-80-bug-fixes)

### Why a language, not a library

- [samber/lo Has 21K Stars. Here's What It Would Look Like as a Language Feature](https://martianov.dev/samber-lo-has-21k-stars-here-s-what-it-would-look-like-as-a-language-feature)
- [Library vs Language: Two Approaches to Functional Programming in Go](https://martianov.dev/library-vs-language-two-approaches-to-functional-programming-in-go)
- [Pattern Matching in Go: Sealed Types and Exhaustive Matching for the Go Ecosystem](https://martianov.dev/pattern-matching-in-go-how-gala-brings-sealed-types-and-exhaustive-matching-to-the-go-ecosystem)
