

- Create ML Components
- AugmentationSequence
-  AugmentationSequence.BatchedSequence 

Structure

# AugmentationSequence.BatchedSequence

An async sequence that batches an augmentation sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct BatchedSequence
```

Available when `Base` conforms to `Sequence`, `RandomTransformer` conforms to `RandomTransformer`, `RandomNumberGenerator` conforms to `RandomNumberGenerator`, `Base.Element` is `AnnotatedFeature`, and `RandomTransformer.Input` is `RandomTransformer.Output`.

## Topics

### Creating an iterator

func makeAsyncIterator() -> AugmentationSequence&lt;Base, RandomTransformer, RandomNumberGenerator, Annotation>.BatchedSequence.AsyncIterator

Creates the asynchronous iterator that produces batches.

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Batching an augmentation sequence

func batches(ofSize: Int, dropsLastPartialBatch: Bool) -> AugmentationSequence&lt;Base, RandomTransformer, RandomNumberGenerator, Annotation>.BatchedSequence

Batches a augmentation sequence.

