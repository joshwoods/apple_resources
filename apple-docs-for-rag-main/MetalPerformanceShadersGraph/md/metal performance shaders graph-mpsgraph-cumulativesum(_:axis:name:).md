

- Metal Performance Shaders Graph
- MPSGraph
-  cumulativeSum(\_:axis:name:) 

Instance Method

# cumulativeSum(\_:axis:name:)

Computes the cumulative sum of the input tensor along the specified axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func cumulativeSum(
    _ tensor: MPSGraphTensor,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor

`axis`  

The tensor dimension where you compute the cumulative operation

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

