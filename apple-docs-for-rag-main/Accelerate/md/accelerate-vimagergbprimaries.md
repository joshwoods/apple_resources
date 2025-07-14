

- Accelerate
-  vImageRGBPrimaries 

Structure

# vImageRGBPrimaries

A representation of the chromaticity of primaries that define a color space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImageRGBPrimaries
```

## Overview

The `x` and `y` values define the chromaticity of each color primary RGB and the white point according to the CIE 1931 color space. For example, the following code defines the RGB primaries for ITU-R BT.709-5:

```
var rgbPrimaries = vImageRGBPrimaries(
    red_x: 0.64,
    green_x: 0.3,
    blue_x: 0.15,
    white_x: 0.3127,
    red_y: 0.33,
    green_y: 0.6,
    blue_y: 0.06,
    white_y: 0.329)
```

## Topics

### Initializers

init(red_x: Float, green_x: Float, blue_x: Float, white_x: Float, red_y: Float, green_y: Float, blue_y: Float, white_y: Float)

Creates a structure that represents the specified chromaticity of primaries defining a color space.

init()

Creates an empty RGB primaries structure.

### Color primary properties

var red_x: Float

The red `x` value according to the CIE 1931 color space.

var green_x: Float

The green `x` value according to the CIE 1931 color space.

var blue_x: Float

The blue `x` value according to the CIE 1931 color space.

var white_x: Float

The white point `x` value according to the CIE 1931 color space.

var red_y: Float

The red `y` value according to the CIE 1931 color space.

var green_y: Float

The green\_ \_`y` value according to the CIE 1931 color space.

var blue_y: Float

The blue `y` value according to the CIE 1931 color space.

var white_y: Float

The white point `y` value according to the CIE 1931 color space.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating Core Graphics color spaces

func vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(UnsafePointer&lt;vImageRGBPrimaries>, UnsafePointer&lt;vImageTransferFunction>, CGColorRenderingIntent, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;CGColorSpace>!

Creates an RGB color space based on primitives from Y’CbCr specifications.

struct vImageTransferFunction

A transfer function to convert from linear to nonlinear RGB.

func vImageCreateMonochromeColorSpaceWithWhitePointAndTransferFunction(UnsafePointer&lt;vImageWhitePoint>, UnsafePointer&lt;vImageTransferFunction>, CGColorRenderingIntent, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;CGColorSpace>!

Creates a monochrome color space based on primitives from Y’CbCr specifications.

struct vImageWhitePoint

A representation of a white point according to the CIE 1931 color space.

