

- Metal Performance Shaders Graph
- MPSGraph
-  reductionOr(with:axes:name:) 

Instance Method

# reductionOr(with:axes:name:)

Creates a reduction or operation and returns the result tensor.

iOS 15.3+iPadOS 15.3+Mac Catalyst 15.3+macOS 12.2+tvOS 15.3+visionOS 1.0+

``` source
func reductionOr(
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

