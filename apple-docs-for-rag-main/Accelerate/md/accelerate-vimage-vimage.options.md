

- Accelerate
- vImage
-  vImage.Options 

Structure

# vImage.Options

Set flags on vImage operations to specify processing options.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct Options
```

## Topics

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

static let noFlags: vImage.Options

A flag that sets the behavior to the default.

static let printDiagnosticsToConsole: vImage.Options

A flag that prints a debug message if the operation fails.

static let truncateKernel: vImage.Options

A flag that uses only the part of the kernel that overlaps the image.

### Instance Properties

var flags: vImage_Flags

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Type Aliases

typealias StructuringElement

A 2D matrix that represents a morphology kernel.

struct ConvolutionKernel

Constants that describe 1D convolution kernels.

struct ConvolutionKernel2D

A 2D matrix that represents a convolution kernel.

struct DynamicPixelFormat

A buffer that contains pixels with a data type that’s unknown at compile time.

struct Interleaved16Fx2

A two-channel, 16-bit-per-channel, floating-point interleaved buffer.

struct Interleaved16Fx4

A four-channel, 16-bit-per-channel, floating-point interleaved buffer.

struct Interleaved16Ux2

A two-channel, 16-bit-per-channel, unsigned-integer interleaved buffer.

struct Interleaved16Ux4

A four-channel, 16-bit-per-channel, unsigned-integer interleaved buffer.

struct Interleaved8x2

A two-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved8x3

A three-channel, 8-bit-per-channel interleaved buffer.

struct Interleaved8x4

A four-channel, 8-bit-per-channel interleaved buffer.

struct InterleavedFx2

A two-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx3

A three-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct InterleavedFx4

A four-channel, 32-bit-per-channel, floating-point interleaved buffer.

struct MultidimensionalLookupTable

A multidimensional lookup table.

