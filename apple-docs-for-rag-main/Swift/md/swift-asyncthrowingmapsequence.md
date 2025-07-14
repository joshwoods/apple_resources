

- Swift
-  AsyncThrowingMapSequence 

Structure

# AsyncThrowingMapSequence

An asynchronous sequence that maps the given error-throwing closure over the asynchronous sequence’s elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AsyncThrowingMapSequence where Base : AsyncSequence
```

## Topics

### Structures

struct Iterator

The iterator that produces elements of the map sequence.

### Type Aliases

typealias Failure

The type of error produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

  Conforms when `Base` conforms to `AsyncSequence`, `Transformed` conforms to `Copyable`, and `Transformed` conforms to `Escapable`.

- Copyable

  Conforms when `Base` conforms to `AsyncSequence`, `Transformed` conforms to `Copyable`, and `Transformed` conforms to `Escapable`.

- Sendable

  Conforms when `Base` conforms to `Sendable`, `Base` conforms to `AsyncSequence`, `Transformed` conforms to `Copyable`, `Transformed` conforms to `Escapable`, `Transformed` conforms to `Sendable`, and `Base.Element` conforms to `Sendable`.

## See Also

### Transforming a Sequence

func map&lt;Transformed>((Self.Element) async -> Transformed) -> AsyncMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements.

struct AsyncMapSequence

An asynchronous sequence that maps the given closure over the asynchronous sequence’s elements.

func map&lt;Transformed>((Self.Element) async throws -> Transformed) -> AsyncThrowingMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given error-throwing closure over the asynchronous sequence’s elements.

func compactMap&lt;ElementOfResult>((Self.Element) async -> ElementOfResult?) -> AsyncCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

struct AsyncCompactMapSequence

An asynchronous sequence that maps a given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

func compactMap&lt;ElementOfResult>((Self.Element) async throws -> ElementOfResult?) -> AsyncThrowingCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

struct AsyncThrowingCompactMapSequence

An asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

struct AsyncFlatMapSequence

An asynchronous sequence that concatenates the results of calling a given transformation with each element of this sequence.

struct AsyncThrowingFlatMapSequence

An asynchronous sequence that concatenates the results of calling a given error-throwing transformation with each element of this sequence.

func reduce&lt;Result>(Result, (Result, Self.Element) async throws -> Result) async rethrows -> Result

Returns the result of combining the elements of the asynchronous sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) async throws -> Void) async rethrows -> Result

Returns the result of combining the elements of the asynchronous sequence using the given closure, given a mutable initial value.

