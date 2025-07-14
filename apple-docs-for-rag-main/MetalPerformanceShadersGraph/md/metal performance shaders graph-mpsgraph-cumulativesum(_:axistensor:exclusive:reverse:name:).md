

- Metal Performance Shaders Graph
- MPSGraph
-  cumulativeSum(\_:axisTensor:exclusive:reverse:name:) 

Instance Method

# cumulativeSum(\_:axisTensor:exclusive:reverse:name:)

Computes the cumulative sum of the input tensor along the specified axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func cumulativeSum(
    _ tensor: MPSGraphTensor,
    axisTensor: MPSGraphTensor,
    exclusive: Bool,
    reverse: Bool,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor

`axisTensor`  

The tensor dimension where you compute the cumulative operation

`exclusive`  

If true, perform the exclusive cumulative operation, and the first element will be equal to zero

`reverse`  

If true, reverse the direction of the cumulative operation along the specified axis

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

