

- Metal Performance Shaders
- Matrices and Vectors
-  MPSTemporaryMatrix 

Class

# MPSTemporaryMatrix

A matrix allocated on GPU private memory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSTemporaryMatrix : MPSMatrix
```

## Topics

### Initializers

init(commandBuffer: any MTLCommandBuffer, matrixDescriptor: MPSMatrixDescriptor)

### Instance Properties

var readCount: Int

### Type Methods

class func prefetchStorage(with: any MTLCommandBuffer, matrixDescriptorList: [MPSMatrixDescriptor])

## Relationships

### Inherits From

- MPSMatrix

## See Also

### Matrices

class MPSMatrix

A 2D array of data that stores the data's values.

class MPSMatrixDescriptor

A description of attributes used to create an MPS matrix.

