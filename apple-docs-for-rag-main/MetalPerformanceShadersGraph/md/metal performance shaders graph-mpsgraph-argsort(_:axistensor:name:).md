

- Metal Performance Shaders Graph
- MPSGraph
-  argSort(\_:axisTensor:name:) 

Instance Method

# argSort(\_:axisTensor:name:)

Computes the indices that sort the elements of the input tensor along the specified axis.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+

``` source
func argSort(
    _ tensor: MPSGraphTensor,
    axisTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor

`axisTensor`  

The tensor dimension over which you sort the tensor

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object with 32-bit integer data type

