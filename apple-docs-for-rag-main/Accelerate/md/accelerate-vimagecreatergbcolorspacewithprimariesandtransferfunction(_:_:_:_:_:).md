

- Accelerate
-  vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(\_:\_:\_:\_:\_:) 

Function

# vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(\_:\_:\_:\_:\_:)

Creates an RGB color space based on primitives from Y’CbCr specifications.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(
    _ primaries: UnsafePointer,
    _ tf: UnsafePointer,
    _ intent: CGColorRenderingIntent,
    _ flags: vImage_Flags,
    _ error: UnsafeMutablePointer!
) -> Unmanaged!
```

## Parameters 

`primaries`  

A set of x, y tristimulus values that define the color primaries for the RGB color space.

`tf`  

The transfer function to convert from linear RGB (using the above primaries) to nonlinear RGB.

`intent`  

A rendering intent constant that specifies how to handle colors that aren’t within the gamut of the destination color space.

`flags`  

The options to use when performing the operation. This function supports only kvImagePrintDiagnosticsToConsole, which prints diagnostic information to the console in the event of a failure.

`error`  

A pointer to a vImage_Error. The function overwrites the pointer to indicate the success or failure of the operation.

## Return Value

A CGColorSpace with a reference count of one.

## Discussion

Use this function to create a CGColorSpace instance to correspond with a specified set of color primaries and a transfer function. The CGColorSpace instance defines an RGB color space. (A Y’CbCr color space is an RGB color space and a conversion matrix from RGB to Y’CbCr). The color primaries provide the white point in XYZ space, and the transfer function provides the transformation from linear color to nonlinear color that the pixels reside in.

For example, the following code defines the RGB color space for ITU-R BT.709-5:

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

var transferFunction = vImageTransferFunction(
    c0: 1.099,
    c1: 1.0,
    c2: 0.0,
    c3: -0.099,
    gamma: 0.45,
    cutoff: 0.018,
    c4: 4.5,
    c5: 0)

let colorSpace = vImageCreateRGBColorSpaceWithPrimariesAndTransferFunction(
    &rgbPrimaries,
    &transferFunction,
    .defaultIntent,
    vImage_Flags(kvImageNoFlags),
    nil)
```

## See Also

### Creating Core Graphics color spaces

struct vImageRGBPrimaries

A representation of the chromaticity of primaries that define a color space.

struct vImageTransferFunction

A transfer function to convert from linear to nonlinear RGB.

func vImageCreateMonochromeColorSpaceWithWhitePointAndTransferFunction(UnsafePointer&lt;vImageWhitePoint>, UnsafePointer&lt;vImageTransferFunction>, CGColorRenderingIntent, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;CGColorSpace>!

Creates a monochrome color space based on primitives from Y’CbCr specifications.

struct vImageWhitePoint

A representation of a white point according to the CIE 1931 color space.

