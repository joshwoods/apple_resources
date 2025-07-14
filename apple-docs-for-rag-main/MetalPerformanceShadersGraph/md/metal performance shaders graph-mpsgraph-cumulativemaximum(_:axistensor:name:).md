

- Metal Performance Shaders Graph
- MPSGraph
-  cumulativeMaximum(\_:axisTensor:name:) 

Instance Method

# cumulativeMaximum(\_:axisTensor:name:)

Computes the cumulative maximum of the input tensor along the specified axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func cumulativeMaximum(
    _ tensor: MPSGraphTensor,
    axisTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor

`axisTensor`  

The tensor dimension where you compute the cumulative operation

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

