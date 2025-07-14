

- Metal Performance Shaders
- Matrices and Vectors
-  MPSVector 

Class

# MPSVector

A 1D array of data that stores the data's values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSVector : NSObject
```

## Topics

### Initializers

init(buffer: any MTLBuffer, descriptor: MPSVectorDescriptor)

init(buffer: any MTLBuffer, offset: Int, descriptor: MPSVectorDescriptor)

init(device: any MTLDevice, descriptor: MPSVectorDescriptor)

### Instance Properties

var data: any MTLBuffer

var dataType: MPSDataType

var device: any MTLDevice

var length: Int

var vectorBytes: Int

var vectors: Int

var offset: Int

### Instance Methods

func resourceSize() -> Int

func synchronize(on: any MTLCommandBuffer)

## Relationships

### Inherits From

- NSObject

## See Also

### Vectors

class MPSVectorDescriptor

A description of the length and data type of a vector.

class MPSTemporaryVector

A vector allocated on GPU private memory.

