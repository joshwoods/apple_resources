

- Create ML
- MLSplitStrategy
-  MLSplitStrategy.automatic 

Case

# MLSplitStrategy.automatic

Create ML automatically decides how much of your training dataset it uses for a validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
case automatic
```

## Discussion

Create ML typically creates a validation dataset by partitioning up to 10% from the training dataset, depending on its size:

| Training samples | % used for validation |
|------------------|-----------------------|
| \

## See Also

### Partitioning data

case fixed(ratio: Double, seed: Int?)

Create ML uses a portion of your training dataset to create a validation dataset based on the ratio.

func resolve(count: Int) -> (ratio: Double, seed: Int)

Resolves this split strategy for a specific element count.

