

- Core Video
-  kCVPixelFormatContainsAlpha 

Global Variable

# kCVPixelFormatContainsAlpha

A Boolean value where kCFBooleanTrue indicates that the format contains alpha and some images may be considered transparent; kCFBooleanFalse indicates that there is no alpha and images are always opaque.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCVPixelFormatContainsAlpha: CFString
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

let kCVPixelFormatPlanes: CFString

let kCVPixelFormatBlockWidth: CFString

let kCVPixelFormatBlockHeight: CFString

The height, in pixels, of the smallest byte-addressable group of pixels (type `CFNumber`). Assumed to be 1 if this key is not present.

let kCVPixelFormatBitsPerBlock: CFString

let kCVPixelFormatBlockHorizontalAlignment: CFString

The horizontal alignment requirements of this format (type `CFNumber`). For example,the alignment for v210 would be 8 here for the horizontal case to match the standard v210 row alignment value of 48. Assumed to be 1 if this key is not present.

