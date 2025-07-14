

- Accelerate
- vImage
- Data Types and Constants
-  Availability Flags 

API Collection

# Availability Flags

Obtain the availability of particular vImage features.

## Topics

### Constants

var VIMAGE_AFFINETRANSFORM_DOUBLE_IS_AVAILABLE: Int32

Defined as `1` if double-precision affine transforms and related functions are supported on the current architecture and in the current SDK, else undefined. See vImage_AffineTransform_Double for more information.

var VIMAGE_CGAFFINETRANSFORM_IS_AVAILABLE: Int32

Defined as `1` if Core Graphics affine transforms and related functions are supported on the current architecture and in the current SDK, else undefined. See vImage_CGAffineTransform for more information.

## See Also

### Constants

Error codes

Error codes that vImage functions return when an operation fails.

Core Video Image Format Errors

Processing Flags

Set flags on vImage operations to specify processing options.

Dithering Methods

Specify the dithering method some vImage conversion functions use.

Decode Arrays

Specify the decode array constant to use with 16Q12-formatted data.

Buffer Types

Look up buffer type codes vImage conversions provide.

typealias vImageMatrixType

An enumeration of RGB -\> Y’CbCr conversion matrix types.

typealias vImage_WarpInterpolation

Constants for selecting the interpolation mode

