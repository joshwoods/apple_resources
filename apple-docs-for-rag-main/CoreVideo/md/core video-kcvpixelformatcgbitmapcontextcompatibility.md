

- Core Video
-  kCVPixelFormatCGBitmapContextCompatibility 

Global Variable

# kCVPixelFormatCGBitmapContextCompatibility

If true, this format is compatible with Core Graphics bitmap contexts(type `CFBoolean`).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
let kCVPixelFormatCGBitmapContextCompatibility: CFString
```

## See Also

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

