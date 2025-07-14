

- Accelerate
-  kvImageNoFlags 

Global Variable

# kvImageNoFlags

A flag that sets the behavior to the default.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageNoFlags: Int { get }
```

## Mentioned in 

Building a Basic Image-Processing Workflow

## See Also

### Constants

struct Options

Set flags on vImage operations to specify processing options.

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

