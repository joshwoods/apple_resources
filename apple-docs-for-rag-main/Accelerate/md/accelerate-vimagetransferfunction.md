

- Accelerate
-  vImageTransferFunction 

Structure

# vImageTransferFunction

A transfer function to convert from linear to nonlinear RGB.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImageTransferFunction
```

## Overview

The transfer function here is in the style of ITU-R BT.709, and is the inverse operation of what appears in an ICC color profile. For example, the following code defines the transfer function for ITU-R BT.709-5:

```
var transferFunction = vImageTransferFunction(
    c0: 1.099,
    c1: 1.0,
    c2: 0.0,
    c3: -0.099,
    gamma: 0.45,
    cutoff: 0.018,
    c4: 4.5,
    c5: 0)
```

The following is the conversion:

```
if (R >= cutoff) {
    R' = c0 * pow( c1 * R + c2, gamma ) + c3
} 
else {
    R' = c4 * R + c5                             
}
```

## Topics

### Initializers

init(c0: CGFloat, c1: CGFloat, c2: CGFloat, c3: CGFloat, gamma: CGFloat, cutoff: CGFloat, c4: CGFloat, c5: CGFloat)

Creates a structure that represents a transfer function to convert from linear to nonlinear RGB.

init()

Creates an empty transfer function structure.

### Transfer function properties

var c0: CGFloat

The `c0` in the transfer function.

var c1: CGFloat

The `c1` in the transfer function.

var c2: CGFloat

The `c2` in the transfer function.

var c3: CGFloat

The `c3` in the transfer function.

var cutoff: CGFloat

The `cutoff` in the transfer function.

var gamma: CGFloat

The `gamma` in the transfer function.

var c4: CGFloat

The `c4` in the transfer function.

var c5: CGFloat

The `c5` in the transfer function.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating Core Graphics color spaces

func vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(UnsafePointer&lt;vImageRGBPrimaries>, UnsafePointer&lt;vImageTransferFunction>, CGColorRenderingIntent, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;CGColorSpace>!

Creates an RGB color space based on primitives from Y’CbCr specifications.

struct vImageRGBPrimaries

A representation of the chromaticity of primaries that define a color space.

func vImageCreateMonochromeColorSpaceWithWhitePointAndTransferFunction(UnsafePointer&lt;vImageWhitePoint>, UnsafePointer&lt;vImageTransferFunction>, CGColorRenderingIntent, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;CGColorSpace>!

Creates a monochrome color space based on primitives from Y’CbCr specifications.

struct vImageWhitePoint

A representation of a white point according to the CIE 1931 color space.

