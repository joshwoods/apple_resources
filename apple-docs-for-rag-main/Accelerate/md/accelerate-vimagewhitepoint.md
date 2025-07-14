

- Accelerate
-  vImageWhitePoint 

Structure

# vImageWhitePoint

A representation of a white point according to the CIE 1931 color space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImageWhitePoint
```

## Topics

### Initializers

init(white_x: Float, white_y: Float)

Creates a structure that represents a white point according to the CIE 1931 color space.

init()

Creates an empty structure that represents a white point.

### White point properties

var white_x: Float

The white point `x` value according to the CIE 1931 color space.

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

struct vImageRGBPrimaries

A representation of the chromaticity of primaries that define a color space.

struct vImageTransferFunction

A transfer function to convert from linear to nonlinear RGB.

func vImageCreateMonochromeColorSpaceWithWhitePointAndTransferFunction(UnsafePointer&lt;vImageWhitePoint>, UnsafePointer&lt;vImageTransferFunction>, CGColorRenderingIntent, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;CGColorSpace>!

Creates a monochrome color space based on primitives from Y’CbCr specifications.

