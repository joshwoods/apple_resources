

- Core Graphics
-  CGBitmapInfo 

Structure

# CGBitmapInfo

Component information for a bitmap image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
struct CGBitmapInfo
```

## Overview

Applications that store pixel data in memory using ARGB format must take care in how they read data. If the code is not written correctly, it’s possible to misread the data which leads to colors or alpha that appear wrong. The byte order constants specify the byte ordering of pixel formats. To specify byte ordering, use a bitwise OR operator to combine the appropriate constant with the `bitmapInfo` parameter.

## Topics

### Constants

static var alphaInfoMask: CGBitmapInfo

The alpha information mask. Use this to extract alpha information that specifies whether a bitmap contains an alpha channel and how the alpha channel is generated.

static var floatComponents: CGBitmapInfo

The components of a bitmap are floating-point values.

static var byteOrderMask: CGBitmapInfo

The byte ordering of pixel formats.

static var byteOrderDefault: CGBitmapInfo

The default byte order.

static var byteOrder16Little: CGBitmapInfo

16-bit, little endian format.

static var byteOrder32Little: CGBitmapInfo

32-bit, little endian format.

static var byteOrder16Big: CGBitmapInfo

16-bit, big endian format.

static var byteOrder32Big: CGBitmapInfo

32-bit, big endian format.

static var floatInfoMask: CGBitmapInfo

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Examining an Image

var isMask: Bool

Returns whether a bitmap image is an image mask.

var width: Int

Returns the width of a bitmap image, in pixels.

var height: Int

Returns the height of a bitmap image.

var bitsPerComponent: Int

Returns the number of bits allocated for a single color component of a bitmap image.

var bitsPerPixel: Int

Returns the number of bits allocated for a single pixel in a bitmap image.

var bytesPerRow: Int

Returns the number of bytes allocated for a single row of a bitmap image.

var colorSpace: CGColorSpace?

Return the color space for a bitmap image.

var alphaInfo: CGImageAlphaInfo

Returns the alpha channel information for a bitmap image.

enum CGImageAlphaInfo

Storage options for alpha component data.

var dataProvider: CGDataProvider?

Returns the data provider for a bitmap image or image mask.

var decode: UnsafePointer&lt;CGFloat>?

Returns the decode array for a bitmap image.

var shouldInterpolate: Bool

Returns the interpolation setting for a bitmap image.

var renderingIntent: CGColorRenderingIntent

Returns the rendering intent setting for a bitmap image.

var bitmapInfo: CGBitmapInfo

Returns the bitmap information for a bitmap image.

var utType: CFString?

The Universal Type Identifier for the image.

