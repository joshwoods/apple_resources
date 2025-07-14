

- Create ML Components
- AnyTemporalSequence
-  AnyTemporalSequence.AsyncIterator 

Type Alias

# AnyTemporalSequence.AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias AsyncIterator = AnyTemporalIterator.Element>
```

## See Also

### Making an iterator

func makeAsyncIterator() -> AnyTemporalIterator&lt;AnyTemporalSequence&lt;Feature>.Element>

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

