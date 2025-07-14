

- Create ML Components
- AugmentationSequence
- AugmentationSequence.BatchedSequence
-  makeAsyncIterator() 

Instance Method

# makeAsyncIterator()

Creates the asynchronous iterator that produces batches.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func makeAsyncIterator() -> AugmentationSequence.BatchedSequence.AsyncIterator
```

## See Also

### Creating an iterator

typealias Element

The type of element produced by this asynchronous sequence.

