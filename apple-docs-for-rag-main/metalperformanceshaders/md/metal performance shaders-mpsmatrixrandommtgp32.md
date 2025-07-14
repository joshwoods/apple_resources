

- Metal Performance Shaders
-  MPSMatrixRandomMTGP32 

Class

# MPSMatrixRandomMTGP32

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSMatrixRandomMTGP32 : MPSMatrixRandom
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

init(device: any MTLDevice, destinationDataType: MPSDataType, seed: Int)

init(device: any MTLDevice, destinationDataType: MPSDataType, seed: Int, distributionDescriptor: MPSMatrixRandomDistributionDescriptor)

### Instance Methods

func synchronizeState(on: any MTLCommandBuffer)

## Relationships

### Inherits From

- MPSMatrixRandom

