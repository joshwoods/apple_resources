

- Swift
- AsyncThrowingFlatMapSequence
-  AsyncThrowingFlatMapSequence.Iterator 

Structure

# AsyncThrowingFlatMapSequence.Iterator

The iterator that produces elements of the flat map sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Iterator
```

Available when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

## Topics

### Instance Methods

func next() async throws -> SegmentOfResult.Element?

Produces the next element in the flat map sequence.

func next(isolation: isolated (any Actor)?) async throws -> SegmentOfResult.Element?

Produces the next element in the flat map sequence.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol
- Sendable

  Conforms when `Base` conforms to `AsyncSequence`, `SegmentOfResult` conforms to `Sendable`, `SegmentOfResult` conforms to `AsyncSequence`, `Base.AsyncIterator` conforms to `Sendable`, `Base.Element` conforms to `Sendable`, `SegmentOfResult.AsyncIterator` conforms to `Sendable`, and `SegmentOfResult.Element` conforms to `Sendable`.

