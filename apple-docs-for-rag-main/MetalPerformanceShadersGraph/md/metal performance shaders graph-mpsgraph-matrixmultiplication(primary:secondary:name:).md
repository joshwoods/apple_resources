

- Metal Performance Shaders Graph
- MPSGraph
-  matrixMultiplication(primary:secondary:name:) 

Instance Method

# matrixMultiplication(primary:secondary:name:)

Computes the matrix multiplication of 2 input tensors with support for broadcasting.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func matrixMultiplication(
    primary primaryTensor: MPSGraphTensor,
    secondary secondaryTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`primaryTensor`  

The left-hand side tensor.

`secondaryTensor`  

The right-hand side tensor.

`name`  

The name for the operation.

## Return Value

A valid tensor containing the product of the input matrices.

