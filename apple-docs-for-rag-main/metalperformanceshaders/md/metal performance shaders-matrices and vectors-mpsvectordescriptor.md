

- Metal Performance Shaders
- Matrices and Vectors
-  MPSVectorDescriptor 

Class

# MPSVectorDescriptor

A description of the length and data type of a vector.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSVectorDescriptor : NSObject
```

## Topics

### Initializers

init(length: Int, dataType: MPSDataType)

init(length: Int, vectors: Int, vectorBytes: Int, dataType: MPSDataType)

### Instance Properties

var dataType: MPSDataType

var length: Int

var vectorBytes: Int

var vectors: Int

### Type Methods

class func vectorBytes(forLength: Int, dataType: MPSDataType) -> Int

## Relationships

### Inherits From

- NSObject

## See Also

### Vectors

class MPSVector

A 1D array of data that stores the data's values.

class MPSTemporaryVector

A vector allocated on GPU private memory.

