

- Accelerate
-  vImage_CGImageFormat 

Structure

# vImage_CGImageFormat

The description of a Core Graphics image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_CGImageFormat
```

## Mentioned in 

Converting bitmap data between Core Graphics images and vImage buffers

Optimizing image-processing performance

Building a basic image conversion workflow

Transforming an image in three dimensions

Converting chroma-subsampled images

## Overview

This structure describes the ordering and number of the color channels, the size and type of the data in the color channels, and alpha information. This format mirrors the image format descriptors that Core Graphics uses to create objects, such as CGImage and doc://com.apple.documentation/documentation/coregraphics/cgbitmapcontext.

## Topics

### Initializers

init(bitsPerComponent: UInt32, bitsPerPixel: UInt32, colorSpace: Unmanaged&lt;CGColorSpace>!, bitmapInfo: CGBitmapInfo, version: UInt32, decode: UnsafePointer&lt;CGFloat>!, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format.

init?(bitsPerComponent: Int, bitsPerPixel: Int, colorSpace: CGColorSpace, bitmapInfo: CGBitmapInfo, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format with a color space instance and default decode array.

init?(cgImage: CGImage)

Creates a Core Graphics image format of the specified image.

init()

Creates an empty Core Graphics image format.

### Instance properties

var bitsPerComponent: UInt32

The number of bits that represents one channel of data in one pixel.

var bitsPerPixel: UInt32

The number of bits that represents one pixel.

var colorSpace: Unmanaged&lt;CGColorSpace>!

A description of the position of the pixel data in the image, relative to a reference XYZ color space.

var bitmapInfo: CGBitmapInfo

The component information that describes the color channels.

var version: UInt32

The version number.

var decode: UnsafePointer&lt;CGFloat>!

The decode array for the image.

var renderingIntent: CGColorRenderingIntent

A rendering intent constant that specifies how Core Graphics handles colors that aren’t within the destination color space gamut.

var componentCount: Int

The number of color and alpha channels.

## Relationships

### Conforms To

- BitwiseCopyable

