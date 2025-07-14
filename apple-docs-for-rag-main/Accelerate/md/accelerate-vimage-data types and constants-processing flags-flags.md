

- Accelerate
- vImage
- Data Types and Constants
-  Processing Flags 

API Collection

# Processing Flags

Set flags on vImage operations to specify processing options.

## Overview

You can pass multiple flags to a function by adding the flag values together. For example, to leave alpha unchanged and turn off tiling, you can pass:

```
kvImageLeaveAlphaUnchanged + kvImageDoNotTile
```

Three of the flags are mutually exclusive: `kvImageCopyInPlace`, `kvImageBackgroundColorFill`, and `kvImageEdgeExtend`. Never pass more than one of these flag values in the same flag parameter.

When passing flags to a function, do not set values for flags that are not used by the function. If the function requires you to set certain flag values, do so. For example, for the convolution function, you must set exactly one of `kvImageCopyInPlace`, `kvImageBackgroundColorFill`, and `kvImageEdgeExtend`. Otherwise the function may return an error. If you don’t want to set flag values, pass `kvImageNoFlags`.

## Topics

### Constants

struct Options

Set flags on vImage operations to specify processing options.

var kvImageNoFlags: Int

A flag that sets the behavior to the default.

var kvImageLeaveAlphaUnchanged: Int

A flag that restricts the operation to red, green, and blue channels only.

var kvImageDoNotTile: Int

A flag that disables vImage internal tiling routines.

var kvImageHighQualityResampling: Int

A flag that uses a higher-quality, slower resampling filter for geometry operations.

var kvImageGetTempBufferSize: Int

A flag that returns the minimum temporary buffer size for the operation, given the parameters provided.

var kvImagePrintDiagnosticsToConsole: Int

A flag that prints a debug message if the operation fails.

var kvImageNoAllocate: Int

A flag that prevents vImage from allocating additional storage.

var kvImageHDRContent: Int

A flag that uses HDR-aware methods.

var kvImageDoNotClamp: Int

A flag that disables clamping in some conversions to floating-point formats.

var kvImageUseFP16Accumulator: Int

A flag that specifies vImage uses faster but lower-precision internal arithmetic for floating-point 16-bit operations.

### Edging Modes

var kvImageCopyInPlace: Int

A flag that copies the value of the edge pixel in the source to the destination.

var kvImageBackgroundColorFill: Int

A flag that uses the background color for missing pixels.

var kvImageEdgeExtend: Int

A flag that extends the edges of the image infinitely.

var kvImageTruncateKernel: Int

A flag that uses only the part of the kernel that overlaps the image.

## See Also

### Constants

Error codes

Error codes that vImage functions return when an operation fails.

Core Video Image Format Errors

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

