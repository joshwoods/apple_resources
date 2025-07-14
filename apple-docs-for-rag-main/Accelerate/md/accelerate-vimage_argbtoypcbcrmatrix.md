

- Accelerate
-  vImage_ARGBToYpCbCrMatrix 

Structure

# vImage_ARGBToYpCbCrMatrix

The 3 x 3 matrix that the vImage library uses to convert from RGB to YpCbCr.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_ARGBToYpCbCrMatrix
```

## Overview

The vImage library uses this matrix to convert from RGB to YpCbCr using the following multiplication:

```
        | Y' |   | R_Yp        G_Yp   B_Yp      |   | R |
        | Cb | = | R_Cb        G_Cb   B_Cb_R_Cr | * | G |
        | Cr |   | B_Cb_R_Cr   G_Cr   B_Cr      |   | B |
```

## Topics

### Creating a conversion matrix

init(R_Yp: Float, G_Yp: Float, B_Yp: Float, R_Cb: Float, G_Cb: Float, B_Cb_R_Cr: Float, G_Cr: Float, B_Cr: Float)

Creates a 3 x 3 matrix for converting RGB to Y’CbCr.

init()

Creates a 3 x 3 zero matrix for converting RGB to Y’CbCr.

### Conversion matrix elements

var R_Yp: Float

The *R_Yp* value in the conversion matrix.

var G_Yp: Float

The *G_Yp* value in the conversion matrix.

var B_Yp: Float

The *B_Yp* value in the conversion matrix.

var R_Cb: Float

The *R_Cb* value in the conversion matrix.

var G_Cb: Float

The *G_Cb* value in the conversion matrix.

var B_Cb_R_Cr: Float

The *B_Cb_R_Cr* value in the conversion matrix.

var G_Cr: Float

The *G_Cr* value in the conversion matrix.

var B_Cr: Float

The *B_Cr* value in the conversion matrix.

### Conversion matrices

var kvImage_ARGBToYpCbCrMatrix_ITU_R_709_2: UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!

RGB-to-Y’CbCr conversion matrix for ITU Recommendation BT.709-2.

var kvImage_ARGBToYpCbCrMatrix_ITU_R_601_4: UnsafePointer&lt;vImage_ARGBToYpCbCrMatrix>!

RGB-to-Y’CbCr conversion matrix for ITU Recommendation BT.601-4.

### Type Properties

static let itu_R_601_4: vImage_ARGBToYpCbCrMatrix

static let itu_R_709_2: vImage_ARGBToYpCbCrMatrix

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

struct vImage_ARGBToYpCbCr

The information that describes the conversion from ARGB to YpCbCr.

struct vImage_YpCbCrPixelRange

The description of range and clamping information for YpCbCr pixel formats.

