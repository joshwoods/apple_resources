

- Metal Performance Shaders Graph
- MPSGraph
-  topKGradient(\_:source:axisTensor:kTensor:name:) 

Instance Method

# topKGradient(\_:source:axisTensor:kTensor:name:)

Creates a TopKGradient operation and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func topKGradient(
    _ gradient: MPSGraphTensor,
    source: MPSGraphTensor,
    axisTensor: MPSGraphTensor,
    kTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

Tensor containing the incoming gradient.

`source`  

Tensor containing source data.

`axisTensor`  

Tensor containing the dimension along which to compute the TopK values.

`kTensor`  

Tensor of the number of largest values to return.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Finds the K largest values along the minor dimension of the input. The input must have at least K elements along its minor dimension.

