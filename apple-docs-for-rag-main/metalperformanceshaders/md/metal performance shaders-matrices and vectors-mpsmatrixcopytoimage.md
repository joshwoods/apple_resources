

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixCopyToImage 

Class

# MPSMatrixCopyToImage

A kernel that copies matrix data to a Metal Performance Shaders image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MPSMatrixCopyToImage : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, dataLayout: MPSDataLayout)

### Instance Properties

var dataLayout: MPSDataLayout

var sourceMatrixBatchIndex: Int

var sourceMatrixOrigin: MTLOrigin

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceMatrix: MPSMatrix, destinationImage: MPSImage)

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceMatrix: MPSMatrix, destinationImages: [MPSImage])

## Relationships

### Inherits From

- MPSKernel

## See Also

### Matrix Copying Operations

class MPSMatrixCopy

A class that can perform multiple matrix copy operations.

class MPSMatrixCopyDescriptor

A description of multiple matrix copy operations.

class MPSImageCopyToMatrix

A class that copies image data to a matrix.

