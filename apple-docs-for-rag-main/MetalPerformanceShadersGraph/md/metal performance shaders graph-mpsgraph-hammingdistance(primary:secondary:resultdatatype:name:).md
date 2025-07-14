

- Metal Performance Shaders Graph
- MPSGraph
-  HammingDistance(primary:secondary:resultDataType:name:) 

Instance Method

# HammingDistance(primary:secondary:resultDataType:name:)

Computes the hamming distance of two input tensors with support for broadcasting.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func HammingDistance(
    primary primaryTensor: MPSGraphTensor,
    secondary secondaryTensor: MPSGraphTensor,
    resultDataType: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`primaryTensor`  

The first input tensor.

`secondaryTensor`  

The second input tensor.

`resultDataType`  

The datatype of the return MPSGraphTensor. Must be either `MPSDataTypeUInt32` or `MPSDataTypeUInt16`.

`name`  

The name for the operation.

## Return Value

A valid tensor containing the hamming distance between the input tensors.

## Discussion

The hamming distance is computed between 2 sets of vectors and the last dimension(s) of each input tensor is considered a vector.

