

- Accelerate
-  kvImageColorSyncIsAbsent 

Global Variable

# kvImageColorSyncIsAbsent

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageColorSyncIsAbsent: Int { get }
```

## See Also

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

var kvImageCoreVideoIsAbsent: Int

var kvImageInternalError: Int

A serious error occured inside vImage, which prevented vImage from continuing.

var kvImageInvalidCVImageFormat: Int

