

- Metal Performance Shaders Graph
- MPSGraph
-  sliceTensor(\_:dimension:start:length:name:) 

Instance Method

# sliceTensor(\_:dimension:start:length:name:)

Creates a slice operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func sliceTensor(
    _ tensor: MPSGraphTensor,
    dimension dimensionIndex: Int,
    start: Int,
    length: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be sliced.

`dimensionIndex`  

The dimension to slice.

`start`  

The starting index of the slice, can be negative to count from the end of the tensor dimension.

`length`  

The length of the slice.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

