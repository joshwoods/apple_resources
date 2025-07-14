

- Swift
- AsyncMapSequence
-  AsyncMapSequence.Iterator 

Structure

# AsyncMapSequence.Iterator

The iterator that produces elements of the map sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Iterator
```

Available when `Base` conforms to `AsyncSequence`.

## Topics

### Instance Methods

func next() async rethrows -> Transformed?

Produces the next element in the map sequence.

func next(isolation: isolated (any Actor)?) async throws(AsyncMapSequence&lt;Base, Transformed>.Failure) -> Transformed?

Produces the next element in the map sequence.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol
- Sendable

  Conforms when `Base` conforms to `AsyncSequence`, `Transformed` conforms to `Copyable`, `Transformed` conforms to `Escapable`, `Transformed` conforms to `Sendable`, `Base.AsyncIterator` conforms to `Sendable`, and `Base.Element` conforms to `Sendable`.

