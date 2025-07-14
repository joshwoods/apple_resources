

- Create ML Components
- SlidingWindowTransformer
- SlidingWindowTransformer.WindowSequence
-  SlidingWindowTransformer.WindowSequence.Iterator 

Structure

# SlidingWindowTransformer.WindowSequence.Iterator

An async iterator of window sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Iterator
```

Available when `Input` conforms to `Sendable`.

## Topics

### Getting the next element

func next() async throws -> TemporalFeature&lt;SlidingWindowTransformer&lt;Input>.Output>?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Creating an iterator

func makeAsyncIterator() -> SlidingWindowTransformer&lt;Input>.WindowSequence.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

