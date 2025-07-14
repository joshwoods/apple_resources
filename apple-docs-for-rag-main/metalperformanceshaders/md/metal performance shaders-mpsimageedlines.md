

- Metal Performance Shaders
-  MPSImageEDLines 

Class

# MPSImageEDLines

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+

``` source
class MPSImageEDLines : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, gaussianSigma: Float, minLineLength: UInt16, maxLines: Int, detailRatio: UInt16, gradientThreshold: Float, lineErrorThreshold: Float, mergeLocalityThreshold: Float)

### Instance Properties

var clipRectSource: MTLRegion

var detailRatio: UInt16

var gaussianSigma: Float

var gradientThreshold: Float

var lineErrorThreshold: Float

var maxLines: Int

var mergeLocalityThreshold: Float

var minLineLength: UInt16

### Instance Methods

func encode(to: any MTLCommandBuffer, sourceTexture: any MTLTexture, destinationTexture: (any MTLTexture)?, endpointBuffer: any MTLBuffer, endpointOffset: Int)

## Relationships

### Inherits From

- MPSKernel

