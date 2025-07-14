

- Accelerate
-  vImage_YpCbCrPixelRange 

Structure

# vImage_YpCbCrPixelRange

The description of range and clamping information for YpCbCr pixel formats.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_YpCbCrPixelRange
```

## Overview

Y’CbCr formats frequently don’t use the entire representable range available to them to represent image data. While a *full range* video format does use the entire range, a *video range* format often leaves the extrema unused, except perhaps to represent values outside of the standard `Y'=[0,1]` `CbCr = [-0.5,0.5]` range. For example, an 8-bit video range format typically uses the range `[16,235]` for Y’ and `[16,240]` for Cb and Cr.

The following code shows examples of typical Y’CbCr pixel ranges:

```
// The 8-bit pixel range that's unclamped.
let pixelRange = vImage_YpCbCrPixelRange(Yp_bias: 16,
                                         CbCr_bias: 128,
                                         YpRangeMax: 235,
                                         CbCrRangeMax: 240,
                                         YpMax: 255,
                                         YpMin: 0,
                                         CbCrMax: 255,
                                         CbCrMin: 1)

 // The 8-bit pixel range that's clamped to video range.
let pixelRange = vImage_YpCbCrPixelRange(Yp_bias: 16,
                                         CbCr_bias: 128,
                                         YpRangeMax: 265,
                                         CbCrRangeMax: 240,
                                         YpMax: 235,
                                         YpMin: 16,
                                         CbCrMax: 240,
                                         CbCrMin: 16)

// The 8-bit pixel range that's clamped to full range.
let pixelRange = vImage_YpCbCrPixelRange(Yp_bias: 0,
                                         CbCr_bias: 128,
                                         YpRangeMax: 255,
                                         CbCrRangeMax: 255,
                                         YpMax: 255,
                                         YpMin: 1,
                                         CbCrMax: 255,
                                         CbCrMin: 0)
```

The bias is the prebias for YUV to RGB and the postbias for RGB to YUV.

## Topics

### Creating a Pixel Range

init(Yp_bias: Int32, CbCr_bias: Int32, YpRangeMax: Int32, CbCrRangeMax: Int32, YpMax: Int32, YpMin: Int32, CbCrMax: Int32, CbCrMin: Int32)

Returns a structure describing range and clamping information for Y’CbCr pixel formats.

init()

### Pixel Range Properties

var Yp_bias: Int32

The encoding for `Y' = 0.0` for this video format (varies by bit depth).

var CbCr_bias: Int32

The encoding for `{Cb, Cr} = 0.0` for this video format.

var YpRangeMax: Int32

The encoding for `Y' = 1.0` for this video format.

var CbCrRangeMax: Int32

The encoding for `{Cb, Cr} = 0.5` for this video format.

var YpMax: Int32

The encoding for the maximum allowed Y’ value.

var YpMin: Int32

The encoding of the minimum allowed Y’ value.

var CbCrMax: Int32

The encoding of the maximum allowed `{Cb, Cr}` value.

var CbCrMin: Int32

The encoding of the minimum allowed `{Cb, Cr}` value.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Generating conversion information

func vImageConvert_ARGBToYpCbCr_GenerateConversion(UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>, UnsafePointer&lt;vImage_YpCbCrPixelRange>, UnsafeMutablePointer&lt;vImage_ARGBToYpCbCr>, vImageARGBType, vImageYpCbCrType, vImage_Flags) -> vImage_Error

Generates the information that describes the conversion from ARGB to YpCbCr.

struct vImageYpCbCrType

Constants that describe the encoding of a YpCbCr image for conversions between RGB and YpCbCr.

struct vImageARGBType

Constants that describe the encoding of an ARGB image for conversions between RGB and YpCbCr.

struct vImage_ARGBToYpCbCrMatrix

The 3 x 3 matrix that the vImage library uses to convert from RGB to YpCbCr.

struct vImage_ARGBToYpCbCr

The information that describes the conversion from ARGB to YpCbCr.

