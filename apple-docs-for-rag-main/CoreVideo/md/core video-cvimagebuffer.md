

- Core Video
-  CVImageBuffer 

API Collection

# CVImageBuffer

An interface for managing different types of image data.

## Overview

Core Video image buffers provides a convenient interface for managing different types of image data. Pixel buffers and Core Video OpenGL buffers derive from the Core Video image buffer.

## Topics

### Inspecting image buffers

func CVImageBufferGetCleanRect(CVImageBuffer) -> CGRect

Returns the source rectangle of a Core Video image buffer that represents the clean aperture of the buffer in encoded pixels.

func CVImageBufferGetColorSpace(CVImageBuffer) -> Unmanaged&lt;CGColorSpace>?

Returns the color space of a Core Video image buffer.

func CVImageBufferGetDisplaySize(CVImageBuffer) -> CGSize

Returns the nominal output display size, in square pixels, of a Core Video image buffer.

func CVImageBufferGetEncodedSize(CVImageBuffer) -> CGSize

Returns the full encoded dimensions of a Core Video image buffer.

func CVImageBufferIsFlipped(CVImageBuffer) -> Bool

Returns a Boolean value indicating whether the image is vertically flipped.

### Creating color spaces

func CVImageBufferCreateColorSpaceFromAttachments(CFDictionary) -> Unmanaged&lt;CGColorSpace>?

Attempts to create a Core Graphics color space from the image buffer’s attachments that you specify.

### Data types

typealias CVImageBuffer

A reference to a Core Video image buffer.

### Converting between strings and integer code points

func CVColorPrimariesGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video color primaries constant string that you specify.

func CVColorPrimariesGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video color primaries string corresponding to the standard integer code point that you specify.

func CVTransferFunctionGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video transfer function string that you specify.

func CVTransferFunctionGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video transfer function string corresponding to the standard integer code point that you specify.

func CVYCbCrMatrixGetIntegerCodePointForString(CFString?) -> Int32

Returns the standard integer code point corresponding to the Core Video YCbCr matrix string that you specify.

func CVYCbCrMatrixGetStringForIntegerCodePoint(Int32) -> Unmanaged&lt;CFString>?

Returns the Core Video YCbCr matrix string corresponding to the standard integer code point that you specify.

### Constants

Image Buffer Attachment Keys

Keys that describe the attachment types associated with image buffers.

Image Buffer Clean Aperture Keys

Keys that describe the clean aperture of an image buffer.

Image Buffer Pixel Aspect Ratio Keys

Keys that describe the pixel aspect ratio of an image buffer.

Image Buffer Display Dimensions Keys

Keys that describe the display dimensions of an image buffer.

Image Buffer Field Detail Constants

Constants that indicate the field order of interlaced video in an image buffer.

Image Buffer YCbCr Matrix Constants

Constants that indicate the type of conversion matrix Core Video uses when it converts image buffer data from the YCbCr color space to the RGB color space.

Image Buffer Color Primaries Constants

Constants that indicate the color primaries gamut for the image buffer.

Image Buffer Transfer Function Constants

Constants that indicate the transfer function for the image buffer.

Image Buffer Chroma Location Constants

Constants that indicate locations for chroma samples in the image buffer.

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

## See Also

### Related Documentation

Core Video Programming Guide

### Data Processing

CVBuffer

An abstract base class that defines how to interact with data buffers.

CVPixelBuffer

An image buffer that holds pixels in main memory.

CVPixelBufferPool

A utility object for managing a recyclable set of pixel buffer objects.

CVPixelFormatDescription

An API that provides functions and types for defining custom pixel formats.

