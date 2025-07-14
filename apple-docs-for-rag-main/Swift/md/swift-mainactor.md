

- Swift
-  MainActor 

Class

# MainActor

A singleton actor whose executor is equivalent to the main dispatch queue.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@globalActor
final actor MainActor
```

## Topics

### Instance Properties

var unownedExecutor: UnownedSerialExecutor

Retrieve the executor for this actor as an optimized, unowned reference.

### Instance Methods

func enqueue(UnownedJob)

### Type Aliases

typealias ActorType

The type of the shared actor instance that will be used to provide mutually-exclusive access to declarations annotated with the given global actor type.

### Type Properties

static let shared: MainActor

The shared actor instance that will be used to provide mutually-exclusive access to declarations annotated with the given global actor type.

static var sharedUnownedExecutor: UnownedSerialExecutor

Shorthand for referring to the `shared.unownedExecutor` of this global actor.

### Type Methods

static func assumeIsolated&lt;T>(() throws -> T, file: StaticString, line: UInt) rethrows -> T

Assume that the current task is executing on the main actor’s serial executor, or stop program execution.

static func run&lt;T>(resultType: T.Type, body: () throws -> T) async rethrows -> T

Execute the given body closure on the main actor.

### Default Implementations

Actor Implementations

GlobalActor Implementations

## Relationships

### Conforms To

- Actor
- GlobalActor
- Sendable

## See Also

### Actors

protocol Sendable

A thread-safe type whose values can be shared across arbitrary concurrent contexts without introducing a risk of data races.

protocol Actor

Common protocol to which all actors conform.

typealias AnyActor

Common marker protocol providing a shared “base” for both (local) `Actor` and (potentially remote) `DistributedActor` types.

Deprecated

protocol GlobalActor

A type that represents a globally-unique actor that can be used to isolate various declarations anywhere in the program.

typealias ConcurrentValueDeprecated

protocol UnsafeSendable

A type whose values can safely be passed across concurrency domains by copying, but which disables some safety checking at the conformance site.

Deprecated

typealias UnsafeConcurrentValueDeprecated

macro isolation&lt;T>() -> T

Produce a reference to the actor to which the enclosing code is isolated, or `nil` if the code is nonisolated.

func extractIsolation&lt;each Arg, Result>((repeat each Arg) async throws -> Result) -> (any Actor)?

