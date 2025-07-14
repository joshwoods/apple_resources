

- Accelerate
- vImage
- Data Types and Constants
-  Error codes 

API Collection

# Error codes

Error codes that vImage functions return when an operation fails.

## Topics

### Constants

enum Error

An error that occurs during a vImage operation.

var kvImageNoError: Int

The vImage function completed without error.

var kvImageRoiLargerThanInputBuffer: Int

The region of interest, as specified by the `srcOffsetToROI_X` and `srcOffsetToROI_Y` parameters and the height and width of the destination buffer, extends beyond the bottom edge or right edge of the source buffer.

var kvImageInvalidKernelSize: Int

Either the kernel height, the kernel width, or both, are even.

var kvImageInvalidEdgeStyle: Int

The edge style specified is invalid.

var kvImageInvalidOffset_X: Int

The `srcOffsetToROI_X` parameter that specifies the left edge of the region of interest is greater than the width of the source image.

var kvImageInvalidOffset_Y: Int

The `srcOffsetToROI_Y` parameter that specifies the top edge of the region of interest is greater than the height of the source image.

var kvImageMemoryAllocationError: Int

An attempt to allocate memory failed.

var kvImageNullPointerArgument: Int

A pointer parameter is `NULL` and it must not be.

var kvImageInvalidParameter: Int

Invalid parameter.

var kvImageBufferSizeMismatch: Int

The function requires the source and destination buffers to have the same height and the same width, but they do not.

var kvImageUnknownFlagsBit: Int

The flag is not recognized.

var kvImageColorSyncIsAbsent: Int

var kvImageCoreVideoIsAbsent: Int

var kvImageInternalError: Int

A serious error occured inside vImage, which prevented vImage from continuing.

var kvImageInvalidCVImageFormat: Int

var kvImageInvalidImageFormat: Int

var kvImageInvalidImageObject: Int

var kvImageInvalidRowBytes: Int

var kvImageOutOfPlaceOperationRequired: Int

var kvImageUnsupportedConversion: Int

Some lower level conversion APIs only support conversion among a sparse matrix of image formats.

### Core Video Image Format Errors

var kvImageCVImageFormat_NoError: Int

An error code that indicates the conversion completed without error.

var kvImageCVImageFormat_ColorSpace: Int

An error code that indicates the image’s color space is missing.

var kvImageCVImageFormat_ChromaSiting: Int

An error code that indicates the chroma siting information is absent.

var kvImageCVImageFormat_AlphaIsOneHint: Int

A hint that indicates the alpha channel is opaque.

var kvImageCVImageFormat_ConversionMatrix: Int

An error code that indicates the required conversion matrix is absent.

var kvImageCVImageFormat_VideoChannelDescription: Int

An error code that indicates the range and clipping information is missing.

## See Also

### Constants

Core Video Image Format Errors

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

