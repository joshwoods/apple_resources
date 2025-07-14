

- Create ML Components
- HumanBodyActionCounter
- HumanBodyActionCounter.CumulativeSumSequence
-  HumanBodyActionCounter.CumulativeSumSequence.Iterator 

Structure

# HumanBodyActionCounter.CumulativeSumSequence.Iterator

An async iterator of cumulative count sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Getting the next element

func next() async throws -> TemporalFeature&lt;Float>?

Advances to the next element and returns it, or nil if no next element exists.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an iterator

func makeAsyncIterator() -> HumanBodyActionCounter.CumulativeSumSequence.Iterator

Constructs an iterator.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

