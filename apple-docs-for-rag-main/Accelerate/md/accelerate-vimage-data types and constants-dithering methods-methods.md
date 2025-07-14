

- Accelerate
- vImage
- Data Types and Constants
-  Dithering Methods 

API Collection

# Dithering Methods

Specify the dithering method some vImage conversion functions use.

## Topics

### Constants

var kvImageConvert_DitherNone: UInt32

A constant that indicates the conversion will not apply dithering.

var kvImageConvert_DitherOrdered: UInt32

A constant that indicates the conversion will add randomized, pre-computed blue noise to the image.

var kvImageConvert_DitherOrderedReproducible: UInt32

A constant that indicates the conversion will add reproducible, pre-computed blue noise to the image.

var kvImageConvert_DitherFloydSteinberg: UInt32

A constant that indicates the conversion will add Floyd-Steinberg dithering to the image.

var kvImageConvert_DitherAtkinson: UInt32

A constant that indicates the conversion will add Atkinson dithering to the image.

var kvImageConvert_OrderedGaussianBlue: UInt32

A constant that indicates the conversion will distribute the noise according to a Gaussian distribution.

var kvImageConvert_OrderedUniformBlue: UInt32

A constant that indicates the conversion will distribute the noise uniformly.

var kvImageConvert_OrderedNoiseShapeMask: UInt32

## See Also

### Constants

Error codes

Error codes that vImage functions return when an operation fails.

Core Video Image Format Errors

Processing Flags

Set flags on vImage operations to specify processing options.

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

