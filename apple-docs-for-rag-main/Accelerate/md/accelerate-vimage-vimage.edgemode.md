

- Accelerate
- vImage
-  vImage.EdgeMode 

Enumeration

# vImage.EdgeMode

Constants that specify edge modes for convolution operations.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum EdgeMode
```

## Topics

### Enumeration Cases

case copyInPlace

An edge mode that copies the value of the edge pixel in the source to the destination.

case extend

An edge mode that extends the edges of the image infinitely.

case fill(backgroundColor: PixelType)

An edge mode that uses the background color for missing pixels.

case truncateKernel

An edge mode that uses only the part of the kernel that overlaps the image.

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

enum Error

An error that occurs during a vImage operation.

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

