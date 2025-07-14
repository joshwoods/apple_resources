

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixDescriptor 

Class

# MPSMatrixDescriptor

A description of attributes used to create an MPS matrix.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSMatrixDescriptor : NSObject
```

## Overview

Matrix data is assumed to be stored in row-major order.

## Topics

### Initializers

init(rows: Int, columns: Int, matrices: Int, rowBytes: Int, matrixBytes: Int, dataType: MPSDataType)

init(rows: Int, columns: Int, rowBytes: Int, dataType: MPSDataType)

### Methods

init(dimensions: Int, columns: Int, rowBytes: Int, dataType: MPSDataType)

Creates a matrix descriptor with the specified dimensions and data type.

class func rowBytes(fromColumns: Int, dataType: MPSDataType) -> Int

Determines the recommended matrix row stride, in bytes, for a given number of columns.

class func rowBytes(forColumns: Int, dataType: MPSDataType) -> Int

### Properties

var rows: Int

The number of rows in the matrix.

var columns: Int

The number of columns in the matrix.

var dataType: MPSDataType

The type of the values in the matrix.

enum MPSDataType

A value to specify a type of data.

var rowBytes: Int

The stride, in bytes, between corresponding elements of consecutive rows in the matrix.

var matrices: Int

var matrixBytes: Int

## Relationships

### Inherits From

- NSObject

## See Also

### Matrices

class MPSMatrix

A 2D array of data that stores the data's values.

class MPSTemporaryMatrix

A matrix allocated on GPU private memory.

