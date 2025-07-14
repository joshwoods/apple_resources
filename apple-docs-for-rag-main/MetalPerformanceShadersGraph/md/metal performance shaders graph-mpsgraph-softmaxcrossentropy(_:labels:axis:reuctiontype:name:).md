

- Metal Performance Shaders Graph
- MPSGraph
-  softMaxCrossEntropy(\_:labels:axis:reuctionType:name:) 

Instance Method

# softMaxCrossEntropy(\_:labels:axis:reuctionType:name:)

Creates a softmax cross-entropy loss operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func softMaxCrossEntropy(
    _ sourceTensor: MPSGraphTensor,
    labels labelsTensor: MPSGraphTensor,
    axis: Int,
    reuctionType reductionType: MPSGraphLossReductionType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`sourceTensor`  

The source tensor.

`labelsTensor`  

The labels tensor.

`axis`  

The axis over which the operation computes the softmax reduction.

`reductionType`  

The type of reduction MPSGraph uses to reduce across all other axes than `axis`. See: MPSGraphLossReductionType.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

The softmax cross-entropy operation computes:

```
    loss = reduction( - labels*ln( softmax(source) )), where
    sotfmax(source) = exp(source) / sum( exp(source) ), and
```

the operation performs the reduction over the `axis` dimension.

