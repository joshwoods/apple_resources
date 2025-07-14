

- Metal Performance Shaders Graph
- MPSGraph
-  topK(\_:k:name:) 

Instance Method

# topK(\_:k:name:)

Creates a TopK operation and returns the value and indices tensors

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func topK(
    _ source: MPSGraphTensor,
    k: Int,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`source`  

Tensor containing source data

`k`  

The number of largest values to return

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor array of size 2

## Discussion

Finds the k largest values along the minor dimension of the input. The source must have at least k elements along its minor dimension. The first element of the result array corresponds to the top values, and the second element of the result array corresponds to the indices of the top values.

