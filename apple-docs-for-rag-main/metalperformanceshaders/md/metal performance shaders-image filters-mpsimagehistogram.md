

- Metal Performance Shaders
- Image Filters
-  MPSImageHistogram 

Class

# MPSImageHistogram

A filter that computes the histogram of an image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.13+tvOS 9.0+visionOS 1.0+

``` source
class MPSImageHistogram : MPSKernel
```

## Overview

Typically, you use an `MPSImageHistogram` filter to calculate an image's histogram that is passed to a subsequent filter such as MPSImageHistogramEqualization or MPSImageHistogramSpecification.

Listing 1 shows how you can create a histogram filter to calculate the histogram of the MTLTexture, `sourceTexture`. The filter is passed an instance of MPSImageHistogramInfo that specifies information to compute the histogram for the channels of an image. After encoding, `histogramInfoBuffer` contains the histogram information and can be used for further operations such as equalization or specification.

var histogramInfo = MPSImageHistogramInfo(
    numberOfHistogramEntries: 256,
    histogramForAlpha: false,
    minPixelValue: vector_float4(0,0,0,0),
    maxPixelValue: vector_float4(1,1,1,1))

let calculation = MPSImageHistogram(device: device,
                                    histogramInfo: &amp;histogramInfo)
let bufferLength = calculation.histogramSize(forSourceFormat: sourceTexture.pixelFormat)
let histogramInfoBuffer = device.makeBuffer(length: bufferLength, 
                                            options: [.storageModePrivate])

calculation.encode(to: commandBuffer,
                   sourceTexture: sourceTexture,
                   histogram: histogramInfoBuffer,
                   histogramOffset: 0)

Listing 1 Creating a histogram filter

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

### Methods

init(device: any MTLDevice, histogramInfo: UnsafePointer&lt;MPSImageHistogramInfo>)

Initializes a histogram with specific information.

struct MPSImageHistogramInfo

The information used to compute the histogram channels of an image.

func encode(to: any MTLCommandBuffer, sourceTexture: any MTLTexture, histogram: any MTLBuffer, histogramOffset: Int)

Encodes the filter to a command buffer using a compute command encoder.

func histogramSize(forSourceFormat: MTLPixelFormat) -> Int

The amount of space the histogram will take up in the output buffer.

### Properties

var clipRectSource: MTLRegion

The source rectangle to use when reading data.

var zeroHistogram: Bool

Determines whether to zero-initialize the histogram results.

var histogramInfo: MPSImageHistogramInfo

A structure describing the histogram content.

var minPixelThresholdValue: vector_float4

## Relationships

### Inherits From

- MPSKernel

## See Also

### Histogram Image Filters

class MPSImageHistogramEqualization

A filter that equalizes the histogram of an image.

class MPSImageHistogramSpecification

A filter that performs a histogram specification operation on an image.

