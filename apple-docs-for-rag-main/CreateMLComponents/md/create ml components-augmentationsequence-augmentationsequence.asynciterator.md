

- Create ML Components
- AugmentationSequence
-  AugmentationSequence.AsyncIterator 

Structure

# AugmentationSequence.AsyncIterator

The iterator that produces elements in the augmentation sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct AsyncIterator
```

Available when `Base` conforms to `Sequence`, `RandomTransformer` conforms to `RandomTransformer`, `RandomNumberGenerator` conforms to `RandomNumberGenerator`, `Base.Element` is `AnnotatedFeature`, and `RandomTransformer.Input` is `RandomTransformer.Output`.

## Topics

### Getting the next element

func next() async throws -> Base.Element?

Produces the next element in the augmentation sequence.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

