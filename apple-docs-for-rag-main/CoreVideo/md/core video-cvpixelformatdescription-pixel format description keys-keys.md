

- Core Video
- CVPixelFormatDescription
-  Pixel Format Description Keys 

API Collection

# Pixel Format Description Keys

The attributes of a pixel format.

## Overview

If you need to define a custom pixel format, you must specify these keys in a Core Foundation dictionary. For information about registering your pixel format, see Technical Q&amp;A 1401: Registering Custom Pixel Formats with QuickTime and Core Video.

In most cases you do not need to specify your own pixel format.

## Topics

### Constants

let kCVPixelFormatComponentRange: CFString

let kCVPixelFormatComponentRange_FullRange: CFString

let kCVPixelFormatComponentRange_VideoRange: CFString

let kCVPixelFormatComponentRange_WideRange: CFString

let kCVPixelFormatContainsRGB: CFString

let kCVPixelFormatContainsYCbCr: CFString

let kCVPixelFormatName: CFString

The name of the pixel format (type `CFString`). This should be the same as the codec name you would use in QuickTime.

let kCVPixelFormatConstant: CFString

The pixel format constant for QuickTime.

let kCVPixelFormatCodecType: CFString

The codec type (type `CFString`). For example, `'2vuy'` or `k422YpCbCr8CodecType`.

let kCVPixelFormatFourCC: CFString

The Microsoft FourCC equivalent code for this pixel format (type `CFString`).

let kCVPixelFormatContainsAlpha: CFString

A Boolean value where kCFBooleanTrue indicates that the format contains alpha and some images may be considered transparent; kCFBooleanFalse indicates that there is no alpha and images are always opaque.

let kCVPixelFormatPlanes: CFString

let kCVPixelFormatBlockWidth: CFString

let kCVPixelFormatBlockHeight: CFString

The height, in pixels, of the smallest byte-addressable group of pixels (type `CFNumber`). Assumed to be 1 if this key is not present.

let kCVPixelFormatBitsPerBlock: CFString

let kCVPixelFormatBlockHorizontalAlignment: CFString

The horizontal alignment requirements of this format (type `CFNumber`). For example,the alignment for v210 would be 8 here for the horizontal case to match the standard v210 row alignment value of 48. Assumed to be 1 if this key is not present.

let kCVPixelFormatBlockVerticalAlignment: CFString

The vertical alignment requirements of this format (type `CFNumber`). Assumed to be 1 if this key is not present.

let kCVPixelFormatBlackBlock: CFString

The bit pattern for a block of black pixels (type `CFData`. If this key is absent, black is assumed to be all zeros. If present, this should be `bitsPerPixel` bits long; if `bitsPerPixel` is less than a byte, repeat the bit pattern for the full byte.

let kCVPixelFormatHorizontalSubsampling: CFString

Horizontal subsampling information for this plane (type `CFNumber`). Assumed to be 1 if this key is not present.

let kCVPixelFormatVerticalSubsampling: CFString

Vertical subsampling information for this plane (type `CFNumber`). Assumed to be 1 if this key is not present.

let kCVPixelFormatOpenGLFormat: CFString

The OpenGL format used to describe this image plane (if applicable). See the OpenGL specification for possible values.

let kCVPixelFormatOpenGLType: CFString

The OpenGL type to describe this image plane (if applicable). See the OpenGL specification for possible values.

let kCVPixelFormatOpenGLInternalFormat: CFString

The OpenGL internal format for this pixel format (if applicable). See the OpenGL specification for possible values.

let kCVPixelFormatCGBitmapInfo: CFString

The Core Graphics bitmap information for this pixel format (if applicable).

let kCVPixelFormatQDCompatibility: CFString

If true, this format is compatible with QuickDraw (type `CFBoolean`).

let kCVPixelFormatCGBitmapContextCompatibility: CFString

If true, this format is compatible with Core Graphics bitmap contexts(type `CFBoolean`).

let kCVPixelFormatCGImageCompatibility: CFString

If true, this format is compatible with the `CGImage` type (type `CFBoolean`).

let kCVPixelFormatOpenGLCompatibility: CFString

If true, this format is compatible with OpenGL (type `CFBoolean`).

let kCVPixelFormatOpenGLESCompatibility: CFString

If true, this format is compatible with OpenGLES (type `CFBoolean`).

let kCVPixelFormatFillExtendedPixelsCallback: CFString

A custom extended pixel fill algorithm (type `CFData`). See CVFillExtendedPixelsCallBack and CVFillExtendedPixelsCallBackData for more information.

## See Also

### Constants

Pixel Format Identifiers

Core Video does not provide support for all of these formats; this list defines only their names.

