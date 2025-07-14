

- Accelerate
- vImage
- vImage.Options
-  noFlags 

Type Property

# noFlags

A flag that sets the behavior to the default.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static let noFlags: vImage.Options
```

## See Also

### Related Documentation

var kvImageNoFlags: Int

A flag that sets the behavior to the default.

### Type Properties

static let backgroundColorFill: vImage.Options

A flag that uses the background color for missing pixels.

static let copyInPlace: vImage.Options

A flag that copies the value of the edge pixel in the source to the destination.

static let doNotClamp: vImage.Options

A flag that disables clamping in some conversions to floating-point formats.

static let doNotTile: vImage.Options

A flag that disables vImage internal tiling routines.

static let getTempBufferSize: vImage.Options

A flag that returns the minimum temporary buffer size for the operation, given the parameters provided.

static let hdrContent: vImage.Options

A flag that uses HDR-aware methods.

static let highQualityResampling: vImage.Options

A flag that uses a higher quality, slower resampling filter for geometry operations.

static let imageExtend: vImage.Options

A flag that extends the edges of the image infinitely.

static let leaveAlphaUnchanged: vImage.Options

A flag that restricts the operation to red, green, and blue channels only.

static let noAllocate: vImage.Options

A flag that prevents vImage from allocating additional storage.

static let printDiagnosticsToConsole: vImage.Options

A flag that prints a debug message if the operation fails.

static let truncateKernel: vImage.Options

A flag that uses only the part of the kernel that overlaps the image.

