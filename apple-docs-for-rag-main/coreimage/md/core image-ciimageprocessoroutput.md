

- Core Image
-  CIImageProcessorOutput 

Protocol

# CIImageProcessorOutput

A container for writing image data and information produced by a custom image processor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
protocol CIImageProcessorOutput
```

## Overview

Your app does not define classes that adopt this protocol; Core Image provides an object of this type when applying a custom image processor you create with a CIImageProcessorKernel subclass.

In your image processor class' process(with:arguments:output:) method, use an appropriate property of the provided `CIImageProcessorOutput` object to return processed pixel data to Core Image. For example, if you process the image using a Metal shader, bind the metalTexture property as an attachment in a render pass or as an output texture in a compute pass. Or, if you process the image using a CPU-based routine, write processed pixel data to memory using the the baseAddress pointer. You must provide rendered output to one (and only one) of the properties listed in Providing Output Image Data.

To access input pixel data in your image processor block, see the CIImageProcessorInput class.

## Topics

### Providing Output Image Data

var baseAddress: UnsafeMutableRawPointer

A pointer to CPU memory at which to write output pixel data.

**Required**

var metalTexture: (any MTLTexture)?

A Metal texture to which you can write output pixel data.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer to which you can write output pixel data.

**Required**

var surface: IOSurfaceRef

An IOSurface object to which you can write output pixel data.

**Required**

### Getting Supplemental Information for Image Processing

var region: CGRect

The rectangular region of the output image that your processor must provide.

**Required**

var metalCommandBuffer: (any MTLCommandBuffer)?

A command buffer to use for image processing using Metal.

**Required**

var bytesPerRow: Int

The number of bytes per row of pixels for the output image.

**Required**

var format: CIFormat

The per-pixel data format expected of the output image.

**Required**

### Instance Properties

var digest: UInt64

**Required**

## See Also

### Custom Image Processors

class CIImageProcessorKernel

The abstract class you extend to create custom image processors that can integrate with Core Image workflows.

protocol CIImageProcessorInput

A container of image data and information for use in a custom image processor.

