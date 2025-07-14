

- Swift
-  AsyncThrowingDropWhileSequence 

Structure

# AsyncThrowingDropWhileSequence

An asynchronous sequence which omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct AsyncThrowingDropWhileSequence where Base : AsyncSequence
```

## Topics

### Structures

struct Iterator

The iterator that produces elements of the drop-while sequence.

### Type Aliases

typealias Failure

The type of element produced by this asynchronous sequence.

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

### Excluding Elements

func dropFirst(Int) -> AsyncDropFirstSequence&lt;Self>

Omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

struct AsyncDropFirstSequence

An asynchronous sequence which omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

func drop(while: (Self.Element) async -> Bool) -> AsyncDropWhileSequence&lt;Self>

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

struct AsyncDropWhileSequence

An asynchronous sequence which omits elements from the base sequence until a given closure returns false, after which it passes through all remaining elements.

func drop(while: (Self.Element) async throws -> Bool) -> AsyncThrowingDropWhileSequence&lt;Self>

Omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

func filter((Self.Element) async -> Bool) -> AsyncFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

struct AsyncFilterSequence

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy a given predicate.

func filter((Self.Element) async throws -> Bool) -> AsyncThrowingFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given error-throwing predicate.

struct AsyncThrowingFilterSequence

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given error-throwing predicate.

