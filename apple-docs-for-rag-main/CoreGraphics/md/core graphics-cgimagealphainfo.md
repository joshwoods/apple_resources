

- Core Graphics
-  CGImageAlphaInfo 

Enumeration

# CGImageAlphaInfo

Storage options for alpha component data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGImageAlphaInfo
```

## Overview

A CGImageAlphaInfo constant specifies (1) whether a bitmap contains an alpha channel, (2) where the alpha bits are located in the image data, and (3) whether the alpha value is premultiplied. You can obtain a CGImageAlphaInfo constant for an image by calling the alphaInfo function. (You provide a CGBitmapInfo constant to the function init(width:height:bitsPerComponent:bitsPerPixel:bytesPerRow:space:bitmapInfo:provider:decode:shouldInterpolate:intent:), part of which is a CGImageAlphaInfo constant.)

Alpha blending is accomplished by combining the color components of the source image with the color components of the destination image using the linear interpolation formula, where “source” is one color component of one pixel of the new paint and “destination” is one color component of the background image.

Core Graphics supports premultiplied alpha only for images. You should not premultiply any other color values specified in Core Graphics.

## Topics

### Constants

case first

The alpha component is stored in the most significant bits of each pixel. For example, non-premultiplied ARGB.

case last

The alpha component is stored in the least significant bits of each pixel. For example, non-premultiplied RGBA.

case none

There is no alpha channel.

case noneSkipFirst

There is no alpha channel. If the total size of the pixel is greater than the space required for the number of color components in the color space, the most significant bits are ignored.

case alphaOnly

There is no color data, only an alpha channel.

case noneSkipLast

There is no alpha channel.

case premultipliedFirst

The alpha component is stored in the most significant bits of each pixel and the color components have already been multiplied by this alpha value. For example, premultiplied ARGB.

case premultipliedLast

The alpha component is stored in the least significant bits of each pixel and the color components have already been multiplied by this alpha value. For example, premultiplied RGBA.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

struct CGBitmapInfo

Component information for a bitmap image.

var utType: CFString?

The Universal Type Identifier for the image.

