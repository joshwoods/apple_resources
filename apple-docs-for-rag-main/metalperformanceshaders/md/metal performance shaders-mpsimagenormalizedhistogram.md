

- Metal Performance Shaders
-  MPSImageNormalizedHistogram 

Class

# MPSImageNormalizedHistogram

A filter that computes the normalized histogram of an image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageNormalizedHistogram : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, histogramInfo: UnsafePointer&lt;MPSImageHistogramInfo>)

### Instance Properties

var clipRectSource: MTLRegion

var histogramInfo: MPSImageHistogramInfo

var zeroHistogram: Bool

### Instance Methods

func encode(to: any MTLCommandBuffer, sourceTexture: any MTLTexture, minmaxTexture: any MTLTexture, histogram: any MTLBuffer, histogramOffset: Int)

func histogramSize(forSourceFormat: MTLPixelFormat) -> Int

## Relationships

### Inherits From

- MPSKernel

