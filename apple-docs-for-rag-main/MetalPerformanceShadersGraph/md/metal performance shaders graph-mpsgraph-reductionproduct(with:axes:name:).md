

- Metal Performance Shaders Graph
- MPSGraph
-  reductionProduct(with:axes:name:) 

Instance Method

# reductionProduct(with:axes:name:)

Creates a reduction product operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func reductionProduct(
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

