

- Metal Performance Shaders Graph
- MPSGraph
-  cumulativeProduct(\_:axis:exclusive:reverse:name:) 

Instance Method

# cumulativeProduct(\_:axis:exclusive:reverse:name:)

Computes the cumulative product of the input tensor along the specified axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func cumulativeProduct(
    _ tensor: MPSGraphTensor,
    axis: Int,
    exclusive: Bool,
    reverse: Bool,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor

`axis`  

The tensor dimension where you compute the cumulative operation

`exclusive`  

If true, perform the exclusive cumulative operation, and the first element will be equal to one

`reverse`  

If true, reverse the direction of the cumulative operation along the specified axis

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

