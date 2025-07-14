

- Accelerate
-  kvImageNoAllocate 

Global Variable

# kvImageNoAllocate

A flag that prevents vImage from allocating additional storage.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageNoAllocate: Int { get }
```

## Discussion

When you set this flag, vImage uses the memory provided to the buffer rather than allocating new memory. For example, instead of overwriting a buffer’s data property with a newly allocated pointer to memory, vImage uses the memory pointed to by the data property directly. In other cases, it may cause the function to assume ownership of a buffer, rather than allocating a copy. You are responsible for making sure the buffer that you allocate is large enough to hold the image. Most vImage functions do not allocate memory and assume that the buffer’s data is already allocated, and, in the case of source image buffers, contain valid pixel data.

## See Also

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

var kvImageHDRContent: Int

A flag that uses HDR-aware methods.

var kvImageDoNotClamp: Int

A flag that disables clamping in some conversions to floating-point formats.

var kvImageUseFP16Accumulator: Int

A flag that specifies vImage uses faster but lower-precision internal arithmetic for floating-point 16-bit operations.

