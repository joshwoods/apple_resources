

- Create ML Components
- HumanBodyActionCounter
- HumanBodyActionCounter.CumulativeSumSequence
-  HumanBodyActionCounter.CumulativeSumSequence.AsyncIterator 

Type Alias

# HumanBodyActionCounter.CumulativeSumSequence.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias AsyncIterator = HumanBodyActionCounter.CumulativeSumSequence.Iterator
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> HumanBodyActionCounter.CumulativeSumSequence.Iterator

Constructs an iterator.

struct Iterator

An async iterator of cumulative count sequence.

typealias Feature

The feature type.

