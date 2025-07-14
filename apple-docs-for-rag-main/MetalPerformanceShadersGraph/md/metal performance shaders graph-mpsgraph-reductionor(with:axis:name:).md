

- Metal Performance Shaders Graph
- MPSGraph
-  reductionOr(with:axis:name:) 

Instance Method

# reductionOr(with:axis:name:)

Creates a reduction or operation and returns the result tensor.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
func reductionOr(
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

