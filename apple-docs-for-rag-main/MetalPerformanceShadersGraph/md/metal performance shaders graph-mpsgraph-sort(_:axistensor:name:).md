

- Metal Performance Shaders Graph
- MPSGraph
-  sort(\_:axisTensor:name:) 

Instance Method

# sort(\_:axisTensor:name:)

Sorts the elements of the input tensor along the specified axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func sort(
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

A valid MPSGraphTensor object

