

- Create ML Components
- SlidingWindowTransformer
- SlidingWindowTransformer.WindowSequence
-  SlidingWindowTransformer.WindowSequence.Feature 

Type Alias

# SlidingWindowTransformer.WindowSequence.Feature

The feature type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Feature = [Input]
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> SlidingWindowTransformer&lt;Input>.WindowSequence.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

An async iterator of window sequence.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

