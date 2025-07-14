

- Metal Performance Shaders Graph
- MPSGraph
-  reductionMaximumPropagateNaN(with:axis:name:) 

Instance Method

# reductionMaximumPropagateNaN(with:axis:name:)

Creates a reduction max propagate NaN operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func reductionMaximumPropagateNaN(
    with tensor: MPSGraphTensor,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

Input tensor

`axis`  

Axis of reduction

`name`  

Name for the operation

## Return Value

A valid MPSGraphTensor object.

