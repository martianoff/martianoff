# Hi, I'm Maksim Martianov

SWE at Snowflake | Ex-Twitter, Route4Me

I build programming languages, distributed systems, and developer tools. Currently creating **GALA** -- a functional programming language that transpiles to Go.

## GALA Language

[GALA](https://github.com/martianoff/gala) (Go Alternative Language) adds sealed types, pattern matching, immutability by default, and monadic error handling to Go -- without sacrificing Go's runtime performance or deployment simplicity. Every `.gala` file compiles to readable `.go` code.

```gala
sealed type Shape {
    case Circle(Radius float64)
    case Rectangle(Width float64, Height float64)
}

val area = shape match {
    case Circle(r)       => 3.14159 * r * r
    case Rectangle(w, h) => w * h
}
```

### Showcase Projects

| Project | Description |
|---------|-------------|
| [**gala**](https://github.com/martianoff/gala) | The GALA transpiler -- sealed types, pattern matching, generics, type inference, zero-reflection JSON, async primitives. 46 releases, 216 verification examples, 80+ bug fixes. Built with Go, ANTLR4, and Bazel. |
| [**gala-playground**](https://github.com/martianoff/gala-playground) | Web-based GALA editor with live transpilation, 15 built-in examples, instant compilation, and dark theme. Try it at [gala-playground.fly.dev](https://gala-playground.fly.dev). |
| [**gala-server**](https://github.com/martianoff/gala-server) | Immutable HTTP server library -- builder pattern, 35+ composable filters (auth, CORS, rate limiting, circuit breaker), sealed type enums, zero-reflection JSON, SSE, graceful shutdown. Inspired by Finagle + Echo. |

### Key Features

- **Sealed types** with exhaustive pattern matching -- the compiler verifies you handle every case
- **Immutability by default** -- `val` bindings, immutable collections (Array, List, HashMap, TreeMap, HashSet, TreeSet)
- **Monadic error handling** -- `Option[T]`, `Either[A, B]`, `Try[T]`, `Future[T]` instead of `if err != nil`
- **Zero-reflection JSON codec** -- type-safe serialization via `StructMeta[T]` compiler intrinsic
- **Full Go interop** -- import and use any Go library, call Go functions, implement Go interfaces
- **22x faster compilation** -- batch transpilation with content-addressed caching

### Blog

I write about GALA's design and implementation at [martianov.dev](https://martianov.dev):

- [The State of GALA: March 2026](https://martianov.dev/state-of-gala-march-2026)
- [22x Faster Builds: Inside GALA's Compilation Performance Journey](https://martianov.dev/22x-faster-builds-gala-compilation-performance)
- [Building a Reliable Transpiler: Lessons from 80+ Bug Fixes](https://martianov.dev/building-reliable-transpiler-80-bug-fixes)
- [Pattern Matching in Go: How GALA Brings Sealed Types and Exhaustive Matching to the Go Ecosystem](https://martianov.dev/pattern-matching-in-go-how-gala-brings-sealed-types-and-exhaustive-matching-to-the-go-ecosystem)
