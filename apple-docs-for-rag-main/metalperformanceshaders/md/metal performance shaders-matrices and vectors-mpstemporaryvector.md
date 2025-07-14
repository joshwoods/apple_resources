

- Metal Performance Shaders
- Matrices and Vectors
-  MPSTemporaryVector 

Class

# MPSTemporaryVector

A vector allocated on GPU private memory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSTemporaryVector : MPSVector
```

## Topics

### Initializers

init(commandBuffer: any MTLCommandBuffer, descriptor: MPSVectorDescriptor)

### Instance Properties

var readCount: Int

### Type Methods

class func prefetchStorage(with: any MTLCommandBuffer, descriptorList: [MPSVectorDescriptor])

## Relationships

### Inherits From

- MPSVector

## See Also

### Vectors

class MPSVector

A 1D array of data that stores the data's values.

class MPSVectorDescriptor

A description of the length and data type of a vector.

