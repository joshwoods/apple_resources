

- Accelerate
- vImage
- Data Types and Constants
-  Core Video Image Format Errors 

API Collection

# Core Video Image Format Errors

## Topics

### Type Aliases

typealias vImageCVImageFormatError

Additional error codes for functions that use the vImageCVImageFormatRef

### Constants

var kvImageCVImageFormat_NoError: Int

An error code that indicates the conversion completed without error.

var kvImageCVImageFormat_ConversionMatrix: Int

An error code that indicates the required conversion matrix is absent.

var kvImageCVImageFormat_ChromaSiting: Int

An error code that indicates the chroma siting information is absent.

var kvImageCVImageFormat_ColorSpace: Int

An error code that indicates the image’s color space is missing.

var kvImageCVImageFormat_VideoChannelDescription: Int

An error code that indicates the range and clipping information is missing.

var kvImageCVImageFormat_AlphaIsOneHint: Int

A hint that indicates the alpha channel is opaque.

## See Also

### Constants

Error codes

Error codes that vImage functions return when an operation fails.

Processing Flags

Set flags on vImage operations to specify processing options.

Dithering Methods

Specify the dithering method some vImage conversion functions use.

Availability Flags

Obtain the availability of particular vImage features.

Decode Arrays

Specify the decode array constant to use with 16Q12-formatted data.

Buffer Types

Look up buffer type codes vImage conversions provide.

typealias vImageMatrixType

An enumeration of RGB -\> Y’CbCr conversion matrix types.

typealias vImage_WarpInterpolation

Constants for selecting the interpolation mode

