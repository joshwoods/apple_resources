

- Accelerate
- vImage
-  vImage.Error 

Enumeration

# vImage.Error

An error that occurs during a vImage operation.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum Error
```

## Topics

### Enumeration Cases

case bufferSizeMismatch

An error indicating that the function requires the source and destination buffers to have the same size, but they don’t.

case colorSyncIsAbsent

An error indicating that the ColorSync framework is missing.

case coreVideoIsAbsent

An error indicating that the Core Video framework is missing.

case internalError

A serious error occurred inside vImage, which prevented vImage from continuing.

case invalidCVImageFormat

An error indicating that a Core Video format is invalid.

case invalidEdgeStyle

An error indicating that the specified edge style is invalid.

case invalidImageFormat

An error indicating that a specified Core Graphics or Core Video format is invalid.

case invalidImageObject

An error indicating that a specified Core Graphics image or Core Video pixel buffer is invalid.

case invalidKernelSize

An error indicating that either the kernel height, the kernel width, or both, are even.

case invalidOffset_X

An error indicating that the parameter that specifies the left edge of the region of interest is greater than the width of the source image.

case invalidOffset_Y

An error indicating that the parameter that specifies the top edge of the region of interest is greater than the height of the source image.

case invalidParameter

An error indicating that a function parameter has an invalid value.

case invalidRowBytes

An error indicating that the buffer’s row bytes field is invalid.

case memoryAllocationError

An error indicating that an attempt to allocate memory failed.

case noError

The vImage function completed without error.

case nullPointerArgument

An error indicating that a pointer parameter is `NULL` and it must not be.

case outOfPlaceOperationRequired

An error indicating that the source images and destination images alias the same image data, but must not.

case roiLargerThanInputBuffer

An error indicating that the region of interest extends beyond the bottom edge or right edge of the source buffer.

case unknownFlagsBit

An error indicating that a bit in the flags field isn’t supported.

case unsupportedConversion

An error indicating that the requested conversion isn’t supported.

### Initializers

init(vImageError: vImage_Error)

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum BlendMode

Constants that specify an alpha blending mode.

enum BufferType

Codes that represent vImage buffer types.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

enum CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

enum EdgeMode

Constants that specify edge modes for convolution operations.

enum FloodFillConnectivity

enum Gamma

Describes either a used-defined or constant gamma.

enum MorphologyOperation

Describes which morphology operation to perform.

enum ReflectionAxis

The axis to reflect an image.

enum Rotation

The angle to rotate an image.

enum ShearDirection

The shear direction.

