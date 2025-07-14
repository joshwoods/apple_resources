

- Swift
-  extractIsolation(\_:) 

Function

# extractIsolation(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func extractIsolation(_ fn: @escaping @isolated(any) (repeat each Arg) async throws -> Result) -> (any Actor)?
```

## See Also

### Actors

protocol Sendable

A thread-safe type whose values can be shared across arbitrary concurrent contexts without introducing a risk of data races.

protocol Actor

Common protocol to which all actors conform.

typealias AnyActor

Common marker protocol providing a shared “base” for both (local) `Actor` and (potentially remote) `DistributedActor` types.

Deprecated

actor MainActor

A singleton actor whose executor is equivalent to the main dispatch queue.

protocol GlobalActor

A type that represents a globally-unique actor that can be used to isolate various declarations anywhere in the program.

typealias ConcurrentValueDeprecated

protocol UnsafeSendable

A type whose values can safely be passed across concurrency domains by copying, but which disables some safety checking at the conformance site.

Deprecated

typealias UnsafeConcurrentValueDeprecated

macro isolation&lt;T>() -> T

Produce a reference to the actor to which the enclosing code is isolated, or `nil` if the code is nonisolated.

