

- Metal Performance Shaders Graph
- MPSGraph
-  concatTensor(\_:with:dimension:name:) 

Instance Method

# concatTensor(\_:with:dimension:name:)

Creates a concatenation operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func concatTensor(
    _ tensor: MPSGraphTensor,
    with tensor2: MPSGraphTensor,
    dimension dimensionIndex: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The first tensor to concatenate.

`tensor2`  

The second tensor to concatenate.

`dimensionIndex`  

The dimension to concatenate across, must be in range: `-rank 

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Concatenates two input tensors along the specified dimension. Tensors must be broadcast compatible along all other dimensions, and have the same datatype.

