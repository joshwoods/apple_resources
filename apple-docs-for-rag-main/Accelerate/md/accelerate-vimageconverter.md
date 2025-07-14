

- Accelerate
-  vImageConverter 

Class

# vImageConverter

A description of a conversion from one image format to another.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class vImageConverter
```

## Mentioned in 

Applying color transforms to images with a multidimensional lookup table

Converting chroma-subsampled images

Building a basic image conversion workflow

## Overview

The vImageConverter class is an opaque type that contains information needed to do a rapid conversion from one image type to another.

You use the converter creation functions, for example, vImageConverter_CreateWithCGImageFormat(_:_:_:_:_:), to create instances of converters. Sometimes, there can be an overhead when creating a converter, so create them in advance and reuse them. Converters are thread safe; that is, you can use the same object concurrently in multiple threads.

## Topics

### Instance Properties

var destinationBufferCount: Int

The number of destination buffers written to by the converter.

var sourceBufferCount: Int

The number of source buffers written to by the converter.

### Instance Methods

func convert(source: vImage_Buffer, destination: inout vImage_Buffer, flags: vImage.Options) throws

Converts the pixels in a vImage buffer to another format.

func mustOperateOutOfPlace(source: vImage_Buffer, destination: vImage_Buffer, flags: vImage.Options) throws -> Bool

Determines whether a converter is capable of operating in place.

func destinationBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage destination buffer types, specifying the order of planes.

func sourceBuffers(colorSpace: CGColorSpace) -> [vImage.BufferType?]

Returns a list of vImage source buffer types, specifying the order of planes.

func convert&lt;Src, Dest>(from: vImage.PixelBuffer&lt;Src>, to: vImage.PixelBuffer&lt;Dest>) throws

func convert&lt;F1, F2>(from: [vImage.PixelBuffer&lt;F1>], to: [vImage.PixelBuffer&lt;F2>]) throws

func makeCGToCVPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

func makeCVToCGPixelBuffers(referencing: CVPixelBuffer) throws -> [vImage.PixelBuffer&lt;vImage.DynamicPixelFormat>]

### Type Methods

static func make(sourceFormat: vImageCVImageFormat, destinationFormat: vImage_CGImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImage_CGImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImageCVImageFormat, flags: vImage.Options) throws -> vImageConverter

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

static func make(sourceFormat: vImage_CGImageFormat, destinationFormat: vImage_CGImageFormat, colorConversionInfo: CGColorConversionInfo) throws -> vImageConverter

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Creating a converter

func vImageConverter_CreateWithCGImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

func vImageConverter_CreateWithCGColorConversionInfo(CGColorConversionInfo, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates an any-to-any converter that uses a color conversion information object to convert from one image format to another.

func vImageConverter_CreateForCGToCVImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, vImageCVImageFormat, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

func vImageConverter_CreateForCVToCGImageFormat(vImageCVImageFormat, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

func vImageConverter_CreateWithColorSyncCodeFragment(CFTypeRef, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>!, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter to convert from one vImage Core Graphics image format to another, using custom ColorSync transform.

