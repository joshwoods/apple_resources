

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixCopy 

Class

# MPSMatrixCopy

A class that can perform multiple matrix copy operations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixCopy : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, copyRows: Int, copyColumns: Int, sourcesAreTransposed: Bool, destinationsAreTransposed: Bool)

### Instance Properties

var copyColumns: Int

var copyRows: Int

var destinationsAreTransposed: Bool

var sourcesAreTransposed: Bool

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, copyDescriptor: MPSMatrixCopyDescriptor)

func encode(commandBuffer: any MTLCommandBuffer, copyDescriptor: MPSMatrixCopyDescriptor, rowPermuteIndices: MPSVector?, rowPermuteOffset: Int, columnPermuteIndices: MPSVector?, columnPermuteOffset: Int)

## Relationships

### Inherits From

- MPSKernel

## See Also

### Matrix Copying Operations

class MPSMatrixCopyToImage

A kernel that copies matrix data to a Metal Performance Shaders image.

class MPSMatrixCopyDescriptor

A description of multiple matrix copy operations.

class MPSImageCopyToMatrix

A class that copies image data to a matrix.

