

- Create ML Components
- AugmentationSequence
-  batches(ofSize:dropsLastPartialBatch:) 

Instance Method

# batches(ofSize:dropsLastPartialBatch:)

Batches a augmentation sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func batches(
    ofSize size: Int,
    dropsLastPartialBatch: Bool
) -> AugmentationSequence.BatchedSequence
```

Available when `Base` conforms to `Sequence`, `RandomTransformer` conforms to `RandomTransformer`, `RandomNumberGenerator` conforms to `RandomNumberGenerator`, `Base.Element` is `AnnotatedFeature`, and `RandomTransformer.Input` is `RandomTransformer.Output`.

## Parameters 

`size`  

The number of elements contained in each batch.

`dropsLastPartialBatch`  

A Boolean value representing whether the last batch should be dropped if it has less than `size` elements.

## Return Value

An async sequence of batches.

## See Also

### Batching an augmentation sequence

struct BatchedSequence

An async sequence that batches an augmentation sequence.

