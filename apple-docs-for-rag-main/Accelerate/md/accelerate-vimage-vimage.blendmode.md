

- Accelerate
- vImage
-  vImage.BlendMode 

Enumeration

# vImage.BlendMode

Constants that specify an alpha blending mode.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum BlendMode
```

## Topics

### Enumeration Cases

case darken

Sets each channel of the destination pixel as the darkest value for the corresponding channel of the two source layers.

case lighten

Sets each channel of the destination pixel as the lightest value for the corresponding channel of the two source layers

case multiply

Sets the destination pixel as the product of the corresponding source pixels.

case screen

Sets the destination pixel as the inverted product of the inverted corresponding source pixels.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Enumerations

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

enum Rotation

The angle to rotate an image.

enum ShearDirection

The shear direction.

