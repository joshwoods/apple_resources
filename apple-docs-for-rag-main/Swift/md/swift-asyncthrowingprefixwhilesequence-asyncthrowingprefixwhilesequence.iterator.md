

- Swift
- AsyncThrowingPrefixWhileSequence
-  AsyncThrowingPrefixWhileSequence.Iterator 

Structure

# AsyncThrowingPrefixWhileSequence.Iterator

The iterator that produces elements of the prefix-while sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Iterator
```

Available when `Base` conforms to `AsyncSequence`.

## Topics

### Instance Methods

func next() async throws -> Base.Element?

Produces the next element in the prefix-while sequence.

func next(isolation: isolated (any Actor)?) async throws -> Base.Element?

Produces the next element in the prefix-while sequence.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol
- Sendable

  Conforms when `Base` conforms to `AsyncSequence`, `Base.AsyncIterator` conforms to `Sendable`, and `Base.Element` conforms to `Sendable`.

