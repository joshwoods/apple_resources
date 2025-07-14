

- Metal Performance Shaders Graph
- MPSGraph
-  reductionAnd(with:axis:name:) 

Instance Method

# reductionAnd(with:axis:name:)

Creates a reduction and operation and returns the result tensor.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
func reductionAnd(
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

