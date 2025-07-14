

- Create ML Components
- AugmentationSequence
- AugmentationSequence.BatchedSequence
-  AugmentationSequence.BatchedSequence.Element 

Type Alias

# AugmentationSequence.BatchedSequence.Element

The type of element produced by this asynchronous sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Element = [AugmentationSequence.Element]
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> AugmentationSequence&lt;Base, RandomTransformer, RandomNumberGenerator, Annotation>.BatchedSequence.AsyncIterator

Creates the asynchronous iterator that produces batches.

