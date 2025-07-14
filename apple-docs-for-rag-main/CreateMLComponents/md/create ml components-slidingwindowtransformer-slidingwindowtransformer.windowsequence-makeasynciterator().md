

- Create ML Components
- SlidingWindowTransformer
- SlidingWindowTransformer.WindowSequence
-  makeAsyncIterator() 

Instance Method

# makeAsyncIterator()

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeAsyncIterator() -> SlidingWindowTransformer.WindowSequence.Iterator
```

## Return Value

An instance of the `AsyncIterator` type used to produce elements of the asynchronous sequence.

## See Also

### Creating an iterator

struct Iterator

An async iterator of window sequence.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Feature

The feature type.

