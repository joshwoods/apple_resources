

- Metal Performance Shaders Graph
- MPSGraph
-  softMaxCrossEntropyGradient(\_:source:labels:axis:reuctionType:name:) 

Instance Method

# softMaxCrossEntropyGradient(\_:source:labels:axis:reuctionType:name:)

Creates the gradient of a softmax cross-entropy loss operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func softMaxCrossEntropyGradient(
    _ gradientTensor: MPSGraphTensor,
    source sourceTensor: MPSGraphTensor,
    labels labelsTensor: MPSGraphTensor,
    axis: Int,
    reuctionType reductionType: MPSGraphLossReductionType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradientTensor`  

The input gradientTensor. Note: in most cases this is the initial gradient tensor, which is a constant tensor with value one.

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

