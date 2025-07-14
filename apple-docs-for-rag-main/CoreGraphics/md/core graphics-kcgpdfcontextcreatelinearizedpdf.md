

- Core Graphics
-  kCGPDFContextCreateLinearizedPDF 

Global Variable

# kCGPDFContextCreateLinearizedPDF

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
let kCGPDFContextCreateLinearizedPDF: CFString
```

## See Also

### Constants

class let colorSpace: CFString

This key specifies the color space of the output buffer. If this key is not included in the dictionary, the output buffer uses the same color space as the display. The value associated with this key must be a CGColorSpace for the desired color space.

Deprecated

class let conversionBlackPointCompensation: CFString

An option for whether to apply black point compensation when converting between color profiles.

var kCGDisplayBitsPerPixel: String

Specifies a CFNumber integer value that represents the number of bits in a pixel.

var kCGDisplayBitsPerSample: String

Specifies a CFNumber integer value that represents the number of bits in an individual sample (for example, a color value in an RGB pixel).

var kCGDisplayBlendNormal: Double

The blend color is not applied at the start or end of a fade operation.

var kCGDisplayBlendSolidColor: Double

The user sees only the blend color at the start or end of a fade operation.

var kCGDisplayBytesPerRow: String

Specifies a CFNumber integer value that represents the number of bytes in a row on the display.

var kCGDisplayFadeReservationInvalidToken: Int32

var kCGDisplayHeight: String

Specifies a CFNumber integer value that represents the height of the display in pixels.

var kCGDisplayIOFlags: String

Specifies a CFNumber integer value that contains the I/O Kit display mode flags. For more information, see the header file `IOKit/IOGraphicsTypes.h`.

var kCGDisplayMode: String

Specifies a `CFNumber` integer value that represents the I/O Kit display mode number.

var kCGDisplayModeIsInterlaced: String

Specifies a CFBoolean value indicating that the I/O Kit interlace mode flag is set.

var kCGDisplayModeIsSafeForHardware: String

Specifies a CFBoolean value indicating that the display mode doesn’t need a confirmation dialog to be set.

Deprecated

var kCGDisplayModeIsStretched: String

Specifies a CFBoolean value indicating that the I/O Kit stretched mode flag is set.

var kCGDisplayModeIsTelevisionOutput: String

Specifies a CFBoolean value indicating that the I/O Kit television output mode flag is set.

