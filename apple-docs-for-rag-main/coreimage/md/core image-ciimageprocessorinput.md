

- Core Image
-  CIImageProcessorInput 

Protocol

# CIImageProcessorInput

A container of image data and information for use in a custom image processor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
protocol CIImageProcessorInput
```

## Overview

Your app does not define classes that adopt this protocol; Core Image provides an object of this type when applying a custom image processor you create with a CIImageProcessorKernel subclass.

In your image processor class' process(with:arguments:output:) method, use the provided `CIImageProcessorInput` object to access the image data and supporting information to perform your custom image processing routine. For example, if you process the image using a Metal shader, use the metalTexture property to bind the image as an input texture. Or, if you process the image using a CPU-based routine, use the baseAddress property to access pixel data in memory.

To finish setting up or performing your image processing routine, use the provided CIImageProcessorOutput object to return processed pixel data to Core Image.

## Topics

### Accessing Input Image Data

var baseAddress: UnsafeRawPointer

A pointer to the image data in CPU memory to be processed.

**Required**

var metalTexture: (any MTLTexture)?

A Metal texture containing the image data to be processed.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer containing the image data to be processed.

**Required**

var surface: IOSurfaceRef

An IOSurface object containing the image data to be processed.

**Required**

### Getting Supplemental Information for Image Processing

var region: CGRect

The area within the input image to be processed.

**Required**

var bytesPerRow: Int

The number of bytes per row of pixels in the input image data.

**Required**

var format: CIFormat

The per-pixel data format of the image to be processed.

**Required**

### Instance Properties

var digest: UInt64

**Required**

var roiTileCount: Int

**Required**

var roiTileIndex: Int

**Required**

## See Also

### Custom Image Processors

class CIImageProcessorKernel

The abstract class you extend to create custom image processors that can integrate with Core Image workflows.

protocol CIImageProcessorOutput

A container for writing image data and information produced by a custom image processor.

