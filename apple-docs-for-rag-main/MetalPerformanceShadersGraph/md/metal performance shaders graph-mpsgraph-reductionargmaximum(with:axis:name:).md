

- Metal Performance Shaders Graph
- MPSGraph
-  reductionArgMaximum(with:axis:name:) 

Instance Method

# reductionArgMaximum(with:axis:name:)

Creates a reduction argMax operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func reductionArgMaximum(
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

