

- Swift
-  AsyncThrowingPrefixWhileSequence 

Structure

# AsyncThrowingPrefixWhileSequence

An asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given error-throwing predicate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AsyncThrowingPrefixWhileSequence where Base : AsyncSequence
```

## Topics

### Structures

struct Iterator

The iterator that produces elements of the prefix-while sequence.

### Type Aliases

typealias Failure

The type of error produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- Copyable

  Conforms when `Base` conforms to `AsyncSequence`.

- Sendable

  Conforms when `Base` conforms to `Sendable`, `Base` conforms to `AsyncSequence`, and `Base.Element` conforms to `Sendable`.

## See Also

### Selecting Elements

func prefix(Int) -> AsyncPrefixSequence&lt;Self>

Returns an asynchronous sequence, up to the specified maximum length, containing the initial elements of the base asynchronous sequence.

struct AsyncPrefixSequence

An asynchronous sequence, up to a specified maximum length, containing the initial elements of a base asynchronous sequence.

func prefix(while: (Self.Element) async -> Bool) rethrows -> AsyncPrefixWhileSequence&lt;Self>

Returns an asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given predicate.

struct AsyncPrefixWhileSequence

An asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy a given predicate.

func prefix(while: (Self.Element) async throws -> Bool) rethrows -> AsyncThrowingPrefixWhileSequence&lt;Self>

Returns an asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given error-throwing predicate.

