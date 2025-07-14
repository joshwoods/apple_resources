

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrix 

Class

# MPSMatrix

A 2D array of data that stores the data's values.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSMatrix : NSObject
```

## Overview

`MPSMatrix` objects serve as inputs and outputs of MPSMatrixMultiplication objects. Matrix data is assumed to be stored in row-major order.

Note

An `MPSMatrix` object maintains its internal storage using a MTLBuffer object. Thus, the same rules for maintaining coherency of the buffer’s data between CPU memory and GPU memory also apply to an `MPSMatrix` object.

## Topics

### Methods

init(buffer: any MTLBuffer, descriptor: MPSMatrixDescriptor)

Initializes a matrix with a buffer.

### Properties

var device: any MTLDevice

The device on which the matrix will be used.

var rows: Int

The number of rows in the matrix.

var columns: Int

The number of columns in the matrix.

var dataType: MPSDataType

The type of the values in the matrix.

var rowBytes: Int

The stride, in bytes, between corresponding elements of consecutive rows in the matrix.

var data: any MTLBuffer

The buffer that stores the matrix data.

var matrices: Int

var matrixBytes: Int

### Initializers

init(buffer: any MTLBuffer, offset: Int, descriptor: MPSMatrixDescriptor)

init(device: any MTLDevice, descriptor: MPSMatrixDescriptor)

### Instance Properties

var offset: Int

### Instance Methods

func resourceSize() -> Int

func synchronize(on: any MTLCommandBuffer)

## Relationships

### Inherits From

- NSObject

## See Also

### Matrices

class MPSMatrixDescriptor

A description of attributes used to create an MPS matrix.

class MPSTemporaryMatrix

A matrix allocated on GPU private memory.

