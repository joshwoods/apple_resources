

- Create ML Components
- AnyTemporalSequence
-  makeAsyncIterator() 

Instance Method

# makeAsyncIterator()

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeAsyncIterator() -> AnyTemporalIterator.Element>
```

## Return Value

An instance of the `AsyncIterator` type used to produce elements of the asynchronous sequence.

## See Also

### Making an iterator

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

