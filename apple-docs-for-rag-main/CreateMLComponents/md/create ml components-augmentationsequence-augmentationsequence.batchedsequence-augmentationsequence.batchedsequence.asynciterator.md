

- Create ML Components
- AugmentationSequence
- AugmentationSequence.BatchedSequence
-  AugmentationSequence.BatchedSequence.AsyncIterator 

Structure

# AugmentationSequence.BatchedSequence.AsyncIterator

The iterator that produces batches.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct AsyncIterator
```

Available when `Base` conforms to `Sequence`, `RandomTransformer` conforms to `RandomTransformer`, `RandomNumberGenerator` conforms to `RandomNumberGenerator`, `Base.Element` is `AnnotatedFeature`, and `RandomTransformer.Input` is `RandomTransformer.Output`.

## Topics

### Getting the next element

func next() async throws -> [AugmentationSequence&lt;Base, RandomTransformer, RandomNumberGenerator, Annotation>.Element]?

Produces the next batch.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

