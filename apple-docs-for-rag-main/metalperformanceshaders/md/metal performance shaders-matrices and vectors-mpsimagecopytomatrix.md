

- Metal Performance Shaders
- Matrices and Vectors
-  MPSImageCopyToMatrix 

Class

# MPSImageCopyToMatrix

A class that copies image data to a matrix.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSImageCopyToMatrix : MPSKernel
```

## Overview

This kernel copies image data to a MPSMatrix object. The image data is stored in a row of a matrix. The dataLayout specifies the order in which the feature channels in the image get stored in the matrix. If the `MPSImage` stores a batch of images, the images are copied into multiple rows, one row per image.

The number of elements in a row in the matrix must be greater than the image width multiplied its height multiplied by the number of featureChannels in the image.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, dataLayout: MPSDataLayout)

### Instance Properties

var dataLayout: MPSDataLayout

var destinationMatrixBatchIndex: Int

var destinationMatrixOrigin: MTLOrigin

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, destinationMatrix: MPSMatrix)

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], destinationMatrix: MPSMatrix)

## Relationships

### Inherits From

- MPSKernel

## See Also

### Matrix Copying Operations

class MPSMatrixCopy

A class that can perform multiple matrix copy operations.

class MPSMatrixCopyToImage

A kernel that copies matrix data to a Metal Performance Shaders image.

class MPSMatrixCopyDescriptor

A description of multiple matrix copy operations.

