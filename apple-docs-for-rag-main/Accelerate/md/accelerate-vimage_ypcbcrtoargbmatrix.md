

- Accelerate
-  vImage_YpCbCrToARGBMatrix 

Structure

# vImage_YpCbCrToARGBMatrix

The 3 x 3 matrix that the vImage library uses to convert from YpCbCr to RGB.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_YpCbCrToARGBMatrix
```

## Overview

The vImage library uses this matrix to convert from YpCbCr to RGB using the following multiplication:

```
                    | R |   | Yp    0     Cr_R |   | Y' |
                    | G | = | Yp   Cb_G   Cr_G | * | Cb |
                    | B |   | Yp   Cb_B     0  |   | Cr |
```

## Topics

### Creating a conversion matrix

init(Yp: Float, Cr_R: Float, Cr_G: Float, Cb_G: Float, Cb_B: Float)

Creates a 3 x 3 matrix for converting Y’CbCr signals to RGB.

init()

Creates a 3 x 3 zero matrix for converting Y’CbCr signals to RGB.

### Conversion matrix elements

var Yp: Float

The *Yp* value in the conversion matrix.

var Cr_R: Float

The *Cr_R* value in the conversion matrix.

var Cr_G: Float

The *Cr_G* value in the conversion matrix.

var Cb_G: Float

The *Cb_G* value in the conversion matrix.

var Cb_B: Float

The *Cb_B* value in the conversion matrix.

### Conversion matrices

var kvImage_YpCbCrToARGBMatrix_ITU_R_601_4: UnsafePointer&lt;vImage_YpCbCrToARGBMatrix>!

Y’CbCr-to-RGB conversion matrix for ITU Recommendation BT.601-4.

var kvImage_YpCbCrToARGBMatrix_ITU_R_709_2: UnsafePointer&lt;vImage_YpCbCrToARGBMatrix>!

Y’CbCr-to-RGB conversion matrix for ITU Recommendation BT.709-2.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Generating conversion information

func vImageConvert_YpCbCrToARGB_GenerateConversion(UnsafePointer&lt;vImage_YpCbCrToARGBMatrix>, UnsafePointer&lt;vImage_YpCbCrPixelRange>, UnsafeMutablePointer&lt;vImage_YpCbCrToARGB>, vImageYpCbCrType, vImageARGBType, vImage_Flags) -> vImage_Error

Generates the information that describes the conversion from YpCbCr to ARGB.

struct vImageYpCbCrType

Constants that describe the encoding of a YpCbCr image for conversions between RGB and YpCbCr.

struct vImageARGBType

Constants that describe the encoding of an ARGB image for conversions between RGB and YpCbCr.

struct vImage_YpCbCrToARGB

The information that describes the conversion from YpCbCr to ARGB.

struct vImage_YpCbCrPixelRange

The description of range and clamping information for YpCbCr pixel formats.

