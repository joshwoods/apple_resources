

- Metal Performance Shaders Graph
- MPSGraph
-  normalizationBetaGradient(withIncomingGradientTensor:sourceTensor:reductionAxes:name:) 

Instance Method

# normalizationBetaGradient(withIncomingGradientTensor:sourceTensor:reductionAxes:name:)

Creates a normalization beta-gradient operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func normalizationBetaGradient(
    withIncomingGradientTensor incomingGradientTensor: MPSGraphTensor,
    sourceTensor: MPSGraphTensor,
    reductionAxes axes: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradientTensor`  

The incoming original `resultTensor` gradient.

`sourceTensor`  

The original input source in forward direction.

`axes`  

The axes of normalization.

`name`  

An optional name for the operation.

## Return Value

A valid `MPSGraphTensor` object.

## Discussion

The mean and variance tensors should be outputs of `meanWithTensor:axes:name` and `varianceWithTensor:meanTensor:axes:name`. Use the axes parameter to achieve different types of normalizations. For example (assuming your data is in `NxHxWxC` format) Batch normalization: axes = \[0, 1, 2\] Instance normalization: axes = \[1, 2\]

