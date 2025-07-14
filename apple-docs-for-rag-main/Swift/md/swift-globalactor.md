

- Swift
-  GlobalActor 

Protocol

# GlobalActor

A type that represents a globally-unique actor that can be used to isolate various declarations anywhere in the program.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol GlobalActor
```

## Overview

A type that conforms to the `GlobalActor` protocol and is marked with the `@globalActor` attribute can be used as a custom attribute. Such types are called global actor types, and can be applied to any declaration to specify that such types are isolated to that global actor type. When using such a declaration from another actor (or from nonisolated code), synchronization is performed through the shared actor instance to ensure mutually-exclusive access to the declaration.

## Custom Actor Executors

A global actor uses a custom executor if it needs to customize its execution semantics, for example, by making sure all of its invocations are run on a specific thread or dispatch queue.

This is done the same way as with normal non-global actors, by declaring a unownedExecutor nonisolated property in the ActorType underlying this global actor.

It is *not* necessary to override the sharedUnownedExecutor static property of the global actor, as its default implementation already delegates to the `shared.unownedExecutor`, which is the most reasonable and correct implementation of this protocol requirement.

You can find out more about custom executors, by referring to the SerialExecutor protocol’s documentation.

See Also

SerialExecutor

## Topics

### Associated Types

associatedtype ActorType : Actor

The type of the shared actor instance that will be used to provide mutually-exclusive access to declarations annotated with the given global actor type.

**Required**

### Type Properties

static var shared: Self.ActorType

The shared actor instance that will be used to provide mutually-exclusive access to declarations annotated with the given global actor type.

**Required**

static var sharedUnownedExecutor: UnownedSerialExecutor

Shorthand for referring to the `shared.unownedExecutor` of this global actor.

**Required** Default implementation provided.

### Type Methods

static func assertIsolated(@autoclosure () -> String, file: StaticString, line: UInt)

Stops program execution if the current task is not executing on this actor’s serial executor.

static func preconditionIsolated(@autoclosure () -> String, file: StaticString, line: UInt)

Stops program execution if the current task is not executing on this actor’s serial executor.

## Relationships

### Conforming Types

- MainActor

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

typealias ConcurrentValueDeprecated

protocol UnsafeSendable

A type whose values can safely be passed across concurrency domains by copying, but which disables some safety checking at the conformance site.

Deprecated

typealias UnsafeConcurrentValueDeprecated

macro isolation&lt;T>() -> T

Produce a reference to the actor to which the enclosing code is isolated, or `nil` if the code is nonisolated.

func extractIsolation&lt;each Arg, Result>((repeat each Arg) async throws -> Result) -> (any Actor)?

