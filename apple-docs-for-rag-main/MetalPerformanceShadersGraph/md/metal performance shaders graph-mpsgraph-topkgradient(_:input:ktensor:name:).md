

- Metal Performance Shaders Graph
- MPSGraph
-  topKGradient(\_:input:kTensor:name:) 

Instance Method

# topKGradient(\_:input:kTensor:name:)

Creates a TopKGradient operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func topKGradient(
    _ gradient: MPSGraphTensor,
    input source: MPSGraphTensor,
    kTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

Tensor containing the incoming gradient.

`source`  

Tensor containing source data.

`kTensor`  

Tensor of the number of largest values to return.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Finds the K largest values along the minor dimension of the input. The input must have at least K elements along its minor dimension.

