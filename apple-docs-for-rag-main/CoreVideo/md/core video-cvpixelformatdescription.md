

- Core Video
-  CVPixelFormatDescription 

API Collection

# CVPixelFormatDescription

An API that provides functions and types for defining custom pixel formats.

## Overview

The Core Video pixel format description API defines functions and types for defining custom pixel formats. You should only use pixel format descriptions if you need to define a custom pixel format.

## Topics

### Creating Format Descriptions

func CVPixelFormatDescriptionCreateWithPixelFormatType(CFAllocator?, OSType) -> CFDictionary?

Creates a pixel format description from a given `OSType` identifier.

func CVPixelFormatDescriptionRegisterDescriptionWithPixelFormatType(CFDictionary, OSType)

Registers a pixel format description with Core Video.

### Retrieving Format Descriptions

func CVPixelFormatDescriptionArrayCreateWithAllPixelFormatTypes(CFAllocator?) -> CFArray?

Returns all the pixel format descriptions known to Core Video.

### Data Types

struct CVFillExtendedPixelsCallBackData

A structure for holding information that describes a custom extended pixel fill algorithm.

### Callbacks

typealias CVFillExtendedPixelsCallBack

Defines a pointer to a custom extended pixel-fill function, which is called whenever the system needs to pad a buffer holding your custom pixel format.

### Constants

Pixel Format Description Keys

The attributes of a pixel format.

Pixel Format Identifiers

Core Video does not provide support for all of these formats; this list defines only their names.

## See Also

### Data Processing

CVBuffer

An abstract base class that defines how to interact with data buffers.

CVImageBuffer

An interface for managing different types of image data.

CVPixelBuffer

An image buffer that holds pixels in main memory.

CVPixelBufferPool

A utility object for managing a recyclable set of pixel buffer objects.

