

- Metal Performance Shaders Graph
- MPSGraph
-  concatTensors(\_:dimension:name:) 

Instance Method

# concatTensors(\_:dimension:name:)

Creates a concatenation operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func concatTensors(
    _ tensors: [MPSGraphTensor],
    dimension dimensionIndex: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensors`  

The tensors to concatenate.

`dimensionIndex`  

The dimension to concatenate across, must be in range: `-rank 

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Concatenates all input tensors along the specified dimension. All inputs must be broadcast compatible along all other dimensions, and have the same datatype.

