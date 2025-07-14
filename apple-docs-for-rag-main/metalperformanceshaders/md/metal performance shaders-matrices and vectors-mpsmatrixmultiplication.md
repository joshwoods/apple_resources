

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixMultiplication 

Class

# MPSMatrixMultiplication

A matrix multiplication kernel.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSMatrixMultiplication : MPSKernel
```

## Overview

An `MPSMatrixMultiplication` object computes the following operation:

*C = alpha \* op(A) \* op(B) + beta \* C*

Where *A*, *B,* and *C* are matrices represented by MPSMatrix objects, and *alpha* and *beta* are scalar values of the same data type as the values of *C*. *A* and *B* may each have an optional transposition operation applied.

Matrices *A*, *B*, and *C* are also referred to as the left input matrix, the right input matrix, and the result matrix respectively.

## Topics

### Methods

init(device: any MTLDevice, transposeLeft: Bool, transposeRight: Bool, resultRows: Int, resultColumns: Int, interiorColumns: Int, alpha: Double, beta: Double)

Initializes a matrix multiplication kernel.

func encode(commandBuffer: any MTLCommandBuffer, leftMatrix: MPSMatrix, rightMatrix: MPSMatrix, resultMatrix: MPSMatrix)

Encodes a matrix multiplication kernel to a command buffer.

### Properties

var leftMatrixOrigin: MTLOrigin

The origin of the left input matrix.

var rightMatrixOrigin: MTLOrigin

The origin of the right input matrix.

var resultMatrixOrigin: MTLOrigin

The origin of the result matrix.

var batchSize: Int

var batchStart: Int

### Initializers

init(device: any MTLDevice, resultRows: Int, resultColumns: Int, interiorColumns: Int)

## Relationships

### Inherits From

- MPSKernel

## See Also

### Matrix Arithmetic Operations

class MPSMatrixSum

A kernel for performing a pointwise summation of a matrix.

class MPSMatrixVectorMultiplication

A matrix-vector multiplication kernel

class MPSMatrixFindTopK

A kernel for computing the top-K values and their corresponding indices in a matrix.

