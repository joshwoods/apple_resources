

- Accelerate
-  kvImageUseFP16Accumulator 

Global Variable

# kvImageUseFP16Accumulator

A flag that specifies vImage uses faster but lower-precision internal arithmetic for floating-point 16-bit operations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var kvImageUseFP16Accumulator: Int { get }
```

## Discussion

Pass this flag to floating-point 16-bit geometry and convolution functions to specify that vImage uses 16-bit floating-point arithmetic. Setting this flag improves performance by up to 2x but at the expense of a less precise result. The loss in precision is typically 2 or 3 bits. However, this may be different for some functions and kernels, and you should verify if a lower-precision arithmetic is suitable for your requirements.

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

var kvImageHDRContent: Int

A flag that uses HDR-aware methods.

var kvImageDoNotClamp: Int

A flag that disables clamping in some conversions to floating-point formats.

