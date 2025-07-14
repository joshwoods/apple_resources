

- Metal Performance Shaders
-  MPSMatrixRandom 

Class

# MPSMatrixRandom

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSMatrixRandom : MPSKernel
```

## Topics

### Instance Properties

var batchSize: Int

var batchStart: Int

var destinationDataType: MPSDataType

var distributionType: MPSMatrixRandomDistribution

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, destinationMatrix: MPSMatrix)

func encode(commandBuffer: any MTLCommandBuffer, destinationVector: MPSVector)

## Relationships

### Inherits From

- MPSKernel

