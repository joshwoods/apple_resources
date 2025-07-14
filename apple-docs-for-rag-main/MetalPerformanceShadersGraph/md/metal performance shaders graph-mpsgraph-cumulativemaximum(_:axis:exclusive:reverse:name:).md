

- Metal Performance Shaders Graph
- MPSGraph
-  cumulativeMaximum(\_:axis:exclusive:reverse:name:) 

Instance Method

# cumulativeMaximum(\_:axis:exclusive:reverse:name:)

Computes the cumulative maximum of the input tensor along the specified axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func cumulativeMaximum(
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

If true, perform the exclusive cumulative operation, and the first element will be equal to the lowest value of the tensor data type

`reverse`  

If true, reverse the direction of the cumulative operation along the specified axis

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

