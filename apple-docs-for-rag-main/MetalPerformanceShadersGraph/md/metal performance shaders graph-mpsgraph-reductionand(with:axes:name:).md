

- Metal Performance Shaders Graph
- MPSGraph
-  reductionAnd(with:axes:name:) 

Instance Method

# reductionAnd(with:axes:name:)

Creates a reduction and operation and returns the result tensor.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
func reductionAnd(
    with tensor: MPSGraphTensor,
    axes: [NSNumber]?,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

Input tensor

`axes`  

Axes of reduction

`name`  

Name for the operation

## Return Value

A valid MPSGraphTensor object.

