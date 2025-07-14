

- Create ML Components
- AnyTemporalSequence
-  AnyTemporalSequence.Element 

Type Alias

# AnyTemporalSequence.Element

The type of element produced by this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Element = TemporalFeature
```

## See Also

### Making an iterator

func makeAsyncIterator() -> AnyTemporalIterator&lt;AnyTemporalSequence&lt;Feature>.Element>

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

