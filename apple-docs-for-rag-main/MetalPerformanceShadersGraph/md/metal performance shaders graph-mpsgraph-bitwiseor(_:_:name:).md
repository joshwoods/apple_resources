

- Metal Performance Shaders Graph
- MPSGraph
-  bitwiseOR(\_:\_:name:) 

Instance Method

# bitwiseOR(\_:\_:name:)

Returns the elementwise bitwise OR of binary representations of two integer tensors.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+

``` source
func bitwiseOR(
    _ primaryTensor: MPSGraphTensor,
    _ secondaryTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`primaryTensor`  

The primary input tensor, must be of integer type.

`secondaryTensor`  

The secondary input tensor, must be of integer type.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

