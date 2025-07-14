

- Accelerate
-  kvImageHDRContent 

Global Variable

# kvImageHDRContent

A flag that uses HDR-aware methods.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var kvImageHDRContent: Int { get }
```

## Discussion

Use this flag in order to provide correct results for input images with pixel values outside the otherwise limited (typically `[-2,2]`) range.

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

var kvImageNoAllocate: Int

A flag that prevents vImage from allocating additional storage.

var kvImageDoNotClamp: Int

A flag that disables clamping in some conversions to floating-point formats.

var kvImageUseFP16Accumulator: Int

A flag that specifies vImage uses faster but lower-precision internal arithmetic for floating-point 16-bit operations.

