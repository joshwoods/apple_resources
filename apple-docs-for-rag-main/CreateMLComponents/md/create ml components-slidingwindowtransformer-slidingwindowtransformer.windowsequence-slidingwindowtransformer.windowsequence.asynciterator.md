

- Create ML Components
- SlidingWindowTransformer
- SlidingWindowTransformer.WindowSequence
-  SlidingWindowTransformer.WindowSequence.AsyncIterator 

Type Alias

# SlidingWindowTransformer.WindowSequence.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias AsyncIterator = SlidingWindowTransformer.WindowSequence.Iterator
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> SlidingWindowTransformer&lt;Input>.WindowSequence.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

An async iterator of window sequence.

typealias Feature

The feature type.

