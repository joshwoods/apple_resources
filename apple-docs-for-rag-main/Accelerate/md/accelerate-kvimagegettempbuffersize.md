

- Accelerate
-  kvImageGetTempBufferSize 

Global Variable

# kvImageGetTempBufferSize

A flag that returns the minimum temporary buffer size for the operation, given the parameters provided.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageGetTempBufferSize: Int { get }
```

## Mentioned in 

Applying geometric transforms to images

## Discussion

When you set this flag, the function returns the number of bytes required for the temporary buffer instead of performing the operation. A negative value indicates an error, and if the function does not accept a temporary buffer, zero is returned.

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

