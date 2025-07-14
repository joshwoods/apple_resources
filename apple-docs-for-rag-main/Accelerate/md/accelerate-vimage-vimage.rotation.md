

- Accelerate
- vImage
-  vImage.Rotation 

Enumeration

# vImage.Rotation

The angle to rotate an image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum Rotation
```

## Topics

### Enumeration Cases

case angleInDegrees(Float)

Rotate by any angle, which you specify in degrees.

case angleInRadians(Float)

Rotate by any angle, which you specify in radians.

case clockwise0Degrees

Rotate 0 degrees (that is, copy without rotating).

case clockwise180Degrees

Rotate 180 degrees clockwise.

case clockwise270Degrees

Rotate 270 degrees clockwise.

case clockwise90Degrees

Rotate 90 degrees clockwise.

case counterClockwise0Degrees

Rotate 0 degrees (that is, copy without rotating).

case counterClockwise180Degrees

Rotate 180 degrees counter-clockwise.

case counterClockwise270Degrees

Rotate 270 degrees counter-clockwise.

case counterClockwise90Degrees

Rotate 90 degrees counter-clockwise.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

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

enum Error

An error that occurs during a vImage operation.

enum FloodFillConnectivity

enum Gamma

Describes either a used-defined or constant gamma.

enum MorphologyOperation

Describes which morphology operation to perform.

enum ReflectionAxis

The axis to reflect an image.

enum ShearDirection

The shear direction.

