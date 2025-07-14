

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixCopyDescriptor 

Class

# MPSMatrixCopyDescriptor

A description of multiple matrix copy operations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixCopyDescriptor : NSObject
```

## Topics

### Initializers

init(device: any MTLDevice, count: Int)

init(sourceMatrices: [MPSMatrix], destinationMatrices: [MPSMatrix], offsetVector: MPSVector?, offset: Int)

init(sourceMatrix: MPSMatrix, destinationMatrix: MPSMatrix, offsets: MPSMatrixCopyOffsets)

### Instance Methods

func setCopyOperationAt(Int, sourceMatrix: MPSMatrix, destinationMatrix: MPSMatrix, offsets: MPSMatrixCopyOffsets)

## Relationships

### Inherits From

- NSObject

## See Also

### Matrix Copying Operations

class MPSMatrixCopy

A class that can perform multiple matrix copy operations.

class MPSMatrixCopyToImage

A kernel that copies matrix data to a Metal Performance Shaders image.

class MPSImageCopyToMatrix

A class that copies image data to a matrix.

